# Arduino PWM — Saída PWM com ledcWrite (ESP32)

🇧🇷 **Português** | 🇺🇸 [English](#english)

---

## Português

Geração de sinal PWM no ESP32 usando a função `ledcWrite` da framework Arduino, com frequência de 10 kHz e resolução de 10 bits.

### O que faz
- Configura o canal PWM 0 a **10 kHz** com **10 bits** de resolução (0–1023)
- Gera saída PWM no **GPIO2**
- Ciclo de trabalho (duty cycle) configurável por software

### Código principal
```cpp
ledcSetup(0, 10000, 10);   // canal 0, 10 kHz, 10 bits
ledcAttachPin(2, 0);        // GPIO2 → canal 0
ledcWrite(0, duty);         // duty cycle 0–1023
```

### Parâmetros
| Parâmetro | Valor |
|---|---|
| Canal LEDC | 0 |
| Frequência | 10.000 Hz |
| Resolução | 10 bits (0–1023) |
| Pino de saída | GPIO2 |

### Plataforma
ESP32 — Arduino Framework

---

## English

PWM signal generation on ESP32 using Arduino's `ledcWrite` function, at 10 kHz frequency and 10-bit resolution.

### What it does
- Configures PWM channel 0 at **10 kHz** with **10-bit** resolution (0–1023)
- Outputs PWM on **GPIO2**
- Duty cycle configurable in software

### Main code
```cpp
ledcSetup(0, 10000, 10);   // channel 0, 10 kHz, 10 bits
ledcAttachPin(2, 0);        // GPIO2 → channel 0
ledcWrite(0, duty);         // duty cycle 0–1023
```

### Parameters
| Parameter | Value |
|---|---|
| LEDC channel | 0 |
| Frequency | 10,000 Hz |
| Resolution | 10 bits (0–1023) |
| Output pin | GPIO2 |

### Platform
ESP32 — Arduino Framework
