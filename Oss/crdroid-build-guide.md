---
tags:
  - Claude
  - Linux
---
# Building crDroid ROM

## Initial Repository Setup

### 1. Create and Navigate to Working Directory
```bash
mkdir -p ~/crdroid
cd ~/crdroid
```

### 2. Initialize crDroid Repository
```bash
repo init -u https://github.com/crdroidandroid/android.git -b 14.0
```

### 3. Sync Source
```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

## Device-Specific Setup

### 1. Device Tree
Create local manifest in `.repo/local_manifests/device.xml`:
```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
  <project name="crdroidandroid/android_device_[manufacturer]_[device]" path="device/[manufacturer]/[device]" remote="github" />
  <project name="crdroidandroid/android_kernel_[manufacturer]_[device]" path="kernel/[manufacturer]/[device]" remote="github" />
  <project name="crdroidandroid/android_vendor_[manufacturer]_[device]" path="vendor/[manufacturer]/[device]" remote="github" />
</manifest>
```

### 2. Sync Device Dependencies
```bash
repo sync --force-sync
```

## Building crDroid

### 1. Setup Build Environment
```bash
source build/envsetup.sh
```

### 2. Select Device Build Configuration
```bash
lunch lineage_[device]-userdebug
```

### 3. Start Build Process
```bash
mka bacon -j$(nproc --all)
```

## crDroid-Specific Customizations

### 1. Common Customization Locations

Key directories for crDroid features:
```
frameworks/base/                    # Core framework modifications
packages/apps/crDroidSettings/     # crDroid specific settings
vendor/lineage/                    # LineageOS-based configurations
vendor/crdroid/                    # crDroid-specific configurations
```

### 2. Popular Modification Areas

1. crDroid Settings
- Location: `packages/apps/crDroidSettings/`
- Contains device-specific features
- UI customization options
- Gesture controls
- Status bar modifications

2. System Modifications
- Quick Settings modifications
- Status bar customizations
- Navigation options
- Screen recording features
- Gaming mode settings

3. Performance Features
- CPU frequency scaling
- GPU performance options
- Thermal profiles
- Battery optimizations

## Testing and Debugging

### 1. Installation
```bash
# Output location: out/target/product/[device]/crDroid-*.zip
# Flash using custom recovery (TWRP/OrangeFox)
```

### 2. Logging
```bash
# Real-time logging
adb logcat | grep -i crdroid

# System logs
adb shell dumpsys > dumpsys.txt
```

## Common crDroid Features to Modify

1. Status Bar
- Quick settings layout
- Clock customization
- Battery style options
- Network traffic monitor

2. Navigation
- Gesture navigation
- Three-button navigation
- Navigation bar customization

3. System
- Screen-off animations
- Power menu customization
- Volume rocker customization
- Screen recording options

4. Theming
- Accent colors
- System fonts
- Icon shapes
- Status bar icons

## Troubleshooting Common Issues

1. Build Errors
- Check crDroid dependencies
- Verify device tree compatibility
- Review vendor blobs

2. Device-Specific Issues
- SELinux policies
- Hardware compatibility
- Vendor modifications

3. Feature Integration
- Proper inheritance from crDroid base
- Resource conflicts
- Framework modifications

## Best Practices

1. Version Control
- Keep track of your modifications
- Document changes in commit messages
- Create separate branches for features

2. Testing
- Test all features thoroughly
- Verify hardware functionality
- Check battery consumption
- Monitor performance metrics

3. Updates
- Regular sync with upstream
- Security patch integration
- Feature backporting when needed