# Hardware (CoreS3 + Matriz 16x16 WS2812)

## Itens
- **M5Stack CoreS3**
- **Matriz LED 16x16 WS2812/WS2812B** (256 LEDs)
- **Fonte 5V (recomendado 8A–15A)** para a matriz (não alimente 256 LEDs pelo USB)
- **Capacitor 1000µF** (entre 5V e GND na entrada da matriz)
- **Resistor 330–470Ω** em série no fio de **DIN**

## Ligação da matriz (recomendado via Grove A)
- **DIN (matriz)** → **GPIO2** (CoreS3 Grove A: fio amarelo)
- **VCC (matriz)** → **5V da fonte externa**
- **GND (matriz)** → **GND da fonte externa**
- **GND do CoreS3** → **GND da fonte externa** (terra comum)

> Se não acender no GPIO2, teste **GPIO1** (ajuste `substitutions: led_pin` no YAML).

## Observações críticas
- **Não alimente a matriz pelo 5V do USB**. 256 LEDs em brilho alto pode passar de **10A**.
- Use **terra comum** (CoreS3 + fonte + matriz).

