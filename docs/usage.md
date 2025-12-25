# Uso

## Matriz (Idle)
No firmware completo (`esphome/voice-assistant-cores3.yaml`), quando estiver ocioso ele alterna:
- **Relógio**
- **Respiração**
- **Clima**

Você pode travar um modo via entidade **`select.voice_assistant_cores3_idle_modo`**.

## Notificações visuais (Home Assistant → CoreS3)
Serviço:
- `esphome.voice_assistant_cores3_notify`

Exemplo (manual):
```yaml
service: esphome.voice_assistant_cores3_notify
data:
  message: "Teste"
  type: "info"
  duration: 5
  priority: 1
```

Tipos suportados: `info`, `warning`, `alert`, `success`, `doorbell`, `alarm`.

## Clima (Home Assistant → CoreS3)
Serviço:
- `esphome.voice_assistant_cores3_update_weather`

As automações em `homeassistant/automations.yaml` já fazem isso a cada 5 minutos usando `weather.home`.

