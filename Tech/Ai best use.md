# Recommended Local AI Models for Fine-tuning

## 1. LLaMA 2 (via Ollama)
### Advantages:
- Best balance of performance and resource requirements
- Extensive community support
- Well-documented fine-tuning process
- Multiple size variants (7B, 13B, 70B)

### Fine-tuning Example:
```bash
# Using Ollama's built-in fine-tuning
ollama create custom-model -f ./Modelfile

# Modelfile example
FROM llama2
SYSTEM "You are a specialized assistant trained on company data"
TEMPLATE "[INST] {{.Prompt}} [/INST]"
```

## 2. Mistral (via Ollama or direct)
### Advantages:
- Superior performance/size ratio
- Lower resource requirements than LLaMA 2
- Modern architecture with better context handling
- Strong reasoning capabilities

### Fine-tuning Example:
```bash
# Using direct fine-tuning
python trainer.py \
  --model_name mistral-7b \
  --dataset custom_data.jsonl \
  --output_dir ./fine_tuned_model \
  --per_device_train_batch_size 4
```

## 3. GPT4All
### Advantages:
- Specifically designed for local deployment
- Very low resource requirements
- Easy integration with custom data
- Active community development

### Fine-tuning Example:
```python
from gpt4all import GPT4All

model = GPT4All("gpt4all-j-v1.3-groovy")
model.fine_tune(
    data_path="training_data.jsonl",
    output_path="fine_tuned_model",
    epochs=3
)
```

## Hardware Requirements

### Minimum Specifications:
- RAM: 16GB (32GB recommended)
- Storage: 100GB SSD
- GPU: 8GB VRAM (16GB recommended)
- CPU: 8 cores (12+ recommended)

### Recommended Setup per Model:
1. LLaMA 2: 32GB RAM, 16GB VRAM
2. Mistral: 24GB RAM, 12GB VRAM
3. GPT4All: 16GB RAM, 8GB VRAM

## Data Preparation Format:
```json
{
    "text": "input text",
    "completion": "expected output",
    "metadata": {
        "source": "internal_docs",
        "category": "technical"
    }
}
```