# voice-models

Custom wake word models for ESPHome / microWakeWord.

## my_wake_word

Trained with [microWakeWord](https://github.com/kahrendt/microWakeWord) locally on Windows + NVIDIA GPU.

**Performance** (quantized streaming TFLite):
- Cutoff 0.93: 2% miss rate, ~0.4 false positives/hour
- Cutoff 0.99: 8% miss rate, ~0.2 false positives/hour

### ESPHome config

```yaml
micro_wake_word:
  models:
    - model: https://raw.githubusercontent.com/BareMetalTinker/voice-models/main/my_wake_word/manifest.json
```
