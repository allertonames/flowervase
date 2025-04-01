---
tags:
  - Linux
  - command
  - sudo
  - install
---
Linux¶

Flathub¶

flatpak install flathub io.kapsa.drive flatpak run io.kapsa.drive 

Build from source¶

sudo apt install flatpak flatpak-builder flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo flatpak install flathub org.freedesktop.Sdk//23.08 flatpak install flathub org.freedesktop.Platform flatpak install org.freedesktop.Sdk.Extension.vala/x86_64/23.08 git clone --recursive git@github.com:flathub/io.kapsa.drive.git cd io.kapsa.drive flatpak-builder --user --install --force-clean build-dir io.kapsa.drive.json 

.deb package¶

wget https://github.com/s3drive/deb-app/releases/latest/download/s3drive_amd64.deb sudo dpkg -i s3drive_amd64.deb 

AppImage¶

wget https://github.com/s3drive/appimage-app/releases/latest/download/S3Drive-x86_64.AppImage chmod +x S3Drive-x86_64.AppImage ./S3Drive-x86_64.AppImage 

Additional requirements¶


Docker

Digital privacy