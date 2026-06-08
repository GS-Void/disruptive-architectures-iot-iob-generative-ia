# 🌌 VOID - Global Solution 2026.1

## 📖 1. Visão Geral

O **VOID** é uma solução disruptiva de monitoramento biométrico para reabilitação física, desenvolvida como projeto da **Global Solution** da disciplina **Disruptive Architectures: IoT, IOB & Generative AI**.

O sistema realiza **telemetria em tempo real** de parâmetros vitais (**BPM** e **Fadiga Muscular**), utilizando sensores integrados a um **ESP32**, processamento em nuvem e dashboards interativos para acompanhamento clínico.

---

## 👥 2. Integrantes (Turma 2TDSPO)

| Integrante                       | RM     |
| -------------------------------- | ------ |
| Pedro Henrique Luiz Alves Duarte | 56349O |
| Guilherme Macedo Martins         | 562396 |
| Henrique Martins                 | 563620 |

---

## 🏗️ 3. Arquitetura da Solução

A solução foi modelada com base em padrões de arquitetura corporativa, garantindo **rastreabilidade** e **escalabilidade**.

### 📡 Camada IoT (Dispositivo)

* ESP32 simulado no **Wokwi**
* Coleta de dados através de sensores analógicos
* Interface com display OLED SSD1306

### 🔗 Camada de Comunicação

* Protocolo **MQTT** para telemetria de baixa latência
* API REST (**HTTP POST**)
* Autenticação **JWT**
* Persistência de dados em ambiente cloud

### ⚙️ Camada de Processamento

* API desenvolvida em **Java**
* Framework **Quarkus**
* Persistência em **Oracle Database**
* Execução em ambiente contêinerizado

### 📊 Camada de Visualização

* Dashboard desenvolvido em **Node-RED**
* Monitoramento em tempo real utilizando:

  * Gauges
  * Donuts
  * Indicadores visuais

---

## 💻 4. Estrutura Técnica

### Firmware

Código desenvolvido em **C++ (Arduino Framework)** utilizando as bibliotecas:

* Adafruit GFX
* Adafruit SSD1306
* PubSubClient

Responsáveis pela interface gráfica e comunicação MQTT do dispositivo.

### Integração

Os dados são enviados simultaneamente para:

* Dashboard em tempo real
* Endpoint de persistência na nuvem

```text
https://java-advanced-5ce0.onrender.com/api/sessoes
```

### 📊 Diagramação

O arquivo `diagram.json` contém toda a topologia do circuito, permitindo a reprodução fiel do ambiente de simulação.

---

## 🚀 5. Guia de Execução

### 1️⃣ Hardware / Simulação

* Acesse o projeto no **Wokwi**
* Inicie a simulação do **ESP32**

### 2️⃣ Dashboard

* Importe o arquivo `flows.json` no **Node-RED**
* Certifique-se de que o broker MQTT esteja ativo:

```text
broker.hivemq.com
```

### 3️⃣ API

O back-end encontra-se operante e pronto para receber requisições **HTTP POST** enviadas pelo dispositivo IoT.

---

## 🎥 6. Demonstração

### 🔗 Link da Simulação

 https://wokwi.com/projects/466198724033639425

### 📹 Vídeo de Apresentação

https://youtu.be/fVzIQKiZows

---

## 🛠️ Tecnologias Utilizadas

* ESP32
* Arduino Framework (C++)
* MQTT
* HiveMQ Broker
* Node-RED
* Java
* Quarkus
* Oracle Database
* JWT Authentication
* Wokwi Simulator
* OLED SSD1306
* Docker

---

## 🎯 Objetivo do Projeto

O VOID foi desenvolvido para fornecer uma solução de monitoramento biométrico inteligente voltada à reabilitação física, permitindo:

* Monitoramento remoto de pacientes
* Coleta de dados em tempo real
* Persistência segura das informações
* Acompanhamento clínico através de dashboards interativos
* Escalabilidade para ambientes hospitalares e centros de reabilitação






