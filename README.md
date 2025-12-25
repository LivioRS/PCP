# Projeto: Assistente (Home Assistant) + M5Stack CoreS3 + Matriz LED 16x16

Este repositório contém um projeto pronto para:
- **M5Stack CoreS3** (ESP32-S3, mic/speaker integrados)
- **Matriz WS2812 16x16 (256 LEDs)** como feedback visual
- **Notificações visuais** disparadas pelo Home Assistant
- **Indicador de clima** (ícone + barra de temperatura)

## Estrutura
- `esphome/led-matrix-test-cores3.yaml`: **teste rápido da matriz**
- `esphome/voice-assistant-cores3.yaml`: **firmware completo (voz + notificações + clima)**
- `esphome/secrets.example.yaml`: modelo do `secrets.yaml`
- `homeassistant/automations.yaml`: exemplos de automações (clima + notificações)
- `homeassistant/scripts.yaml`: script pra enviar notificação manual
- `homeassistant/dashboard.yaml`: dashboard simples (entities)
- `docs/hardware.md`: ligação elétrica e cuidados de energia
- `docs/installation.md`: passo a passo
- `docs/usage.md`: como usar

## Como testar (ordem certa)
1. **Conecte a matriz com fonte externa** (ver `docs/hardware.md`).
2. Flash via USB o `esphome/led-matrix-test-cores3.yaml`.
3. Se acender, flash o `esphome/voice-assistant-cores3.yaml`.

