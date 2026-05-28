# 🌱 SafeSpace — Guardião de Estufa Espacial

## 📌 Sobre o Projeto

O **SafeSpace** é um sistema inteligente de monitoramento para estufas espaciais em habitats lunares ou marcianos.

O projeto foi desenvolvido utilizando:

* ESP32
* TinyML
* Edge Computing
* WebServer embarcado
* Simulação no Wokwi

A solução monitora continuamente:

* temperatura
* umidade
* luminosidade

e classifica automaticamente o ambiente em:

* 🟢 Seguro
* 🟡 Alerta
* 🔴 Crítico

O objetivo é garantir condições ideais para produção de alimentos e manutenção da vida em colônias espaciais.

---

# 🎯 Objetivo

Criar um sistema embarcado inteligente capaz de:

* detectar anomalias ambientais
* emitir alertas locais
* disponibilizar monitoramento remoto via navegador

Tudo isso utilizando inferência leve inspirada em TinyML.

---

# 🌍 ODS Relacionada

## ODS 11 — Cidades e Comunidades Sustentáveis

O projeto contribui para:

* habitats inteligentes
* automação sustentável
* monitoramento ambiental
* resiliência em ambientes extremos

---

# 🧠 TinyML

O modelo TinyML foi treinado utilizando dados simulados exportados em CSV.

Como a versão gratuita do Wokwi não suporta a biblioteca completa do Edge Impulse, as regras aprendidas pelo modelo foram convertidas manualmente em estruturas condicionais (`if/else`) dentro do código C++ do ESP32.

---

# 🛠 Tecnologias Utilizadas

| Tecnologia   | Função                     |
| ------------ | -------------------------- |
| ESP32        | Microcontrolador principal |
| Wokwi        | Simulação do hardware      |
| Edge Impulse | Treinamento TinyML         |
| HTML/CSS     | Dashboard Web              |
| C++          | Programação embarcada      |
| WiFi         | Comunicação local          |

---

# ⚙ Componentes

| Componente      | Função                |
| --------------- | --------------------- |
| ESP32 DevKit V1 | Processamento         |
| DHT22           | Temperatura e umidade |
| LDR             | Luminosidade          |
| LED Verde       | Estado seguro         |
| LED Amarelo     | Estado alerta         |
| LED Vermelho    | Estado crítico        |
| Buzzer          | Alarme sonoro         |

---

# 🚨 Estados do Sistema

| Estado  | Condição            |
| ------- | ------------------- |
| Seguro  | Ambiente ideal      |
| Alerta  | Pequenas anomalias  |
| Crítico | Risco para a estufa |

---

# 🌐 WebServer

O ESP32 hospeda uma página web acessível pela rede local contendo:

* status atual
* temperatura
* umidade
* luminosidade
* atualização automática

---

# 📊 Dataset

O dataset foi gerado artificialmente simulando:

* variações climáticas
* baixa luminosidade
* extremos ambientais

Classes utilizadas:

* seguro
* alerta
* critico

Arquivo:

```txt
dataset/habitat_dataset.csv
```

---

# 📂 Estrutura do Projeto

```txt
SafeSpace/
│
├── README.md
├── diagram.json
├── sketch.ino
│
├── dataset/
│   └── habitat_dataset.csv
│
├── modelo/
│   └── model.h
│
└── video/
    └── demonstracao.mp4
```

---

# ▶ Como Executar

## 1. Abrir o projeto no Wokwi

Importar:

* `diagram.json`
* `sketch.ino`

---

## 2. Iniciar simulação

Clique em:

```txt
Start Simulation
```

---

## 3. Abrir WebServer

Abrir o IP exibido no monitor serial.

Exemplo:

```txt
http://192.168.x.x
```

---

# 🎥 Demonstração

O vídeo demonstra:

* sensores variando
* classificação dos estados
* LEDs
* buzzer
* dashboard web
* monitor serial

---

# 👨‍🚀 Integrantes

| Nome         | RM      |
| ------------ | ------- |
| Integrante 1 | RMXXXXX |
| Integrante 2 | RMXXXXX |
| Integrante 3 | RMXXXXX |

---

# 🚀 Futuras Melhorias

* MQTT
* Node-RED
* Dashboard em nuvem
* IA embarcada real
* múltiplas estufas
* gráficos em tempo real
* detecção preditiva

---

# 📡 Conceito

> “SafeSpace protege habitats agrícolas espaciais através de monitoramento inteligente em tempo real utilizando Edge AI e IoT embarcada.”
