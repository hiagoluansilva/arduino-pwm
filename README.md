# arduino-pwm

Controle de brilho de LED com PWM em fade suave no ESP32 usando a API `ledcWrite`.

## Descrição

Demonstração do controle de duty cycle PWM no ESP32. O brilho de um LED aumenta gradualmente de 0 a 100% e depois diminui de volta, criando um efeito de fade (respiração).

## Hardware

- Placa: ESP32
- LED no pino GPIO 2

## Configuração PWM

| Parâmetro | Valor |
|-----------|-------|
| Canal LEDC | 0 |
| Frequência | 10.000 Hz |
| Resolução | 10 bits (0–1023) |
| Pino | GPIO 2 |

## Como usar

1. Abra `pwm.ino` no Arduino IDE
2. Selecione a placa **ESP32 Dev Module**
3. Compile e grave

## Escola

Centro Tecnológico Liberato — Novo Hamburgo/RS
