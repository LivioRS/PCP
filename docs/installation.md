# Instalação (ESPHome + Home Assistant)

## 1) ESPHome
1. Copie `esphome/secrets.example.yaml` para `esphome/secrets.yaml` e preencha Wi-Fi/API/OTA.
2. No ESPHome Dashboard, adicione o dispositivo e aponte para um destes arquivos:
   - **Teste rápido (só matriz)**: `esphome/led-matrix-test-cores3.yaml`
   - **Completo (voz + notificações + clima)**: `esphome/voice-assistant-cores3.yaml`

## 2) Ordem de teste recomendada
1. Flash do **`led-matrix-test-cores3.yaml`** via USB-C.
2. Confirmou que a matriz acende? Aí sim flash do **`voice-assistant-cores3.yaml`**.

## 3) Home Assistant
1. Integração ESPHome: *Configurações → Dispositivos e Serviços → ESPHome*.
2. Importe/cole as automações de `homeassistant/automations.yaml`.
3. (Opcional) crie um dashboard e cole `homeassistant/dashboard.yaml`.

