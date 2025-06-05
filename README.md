# HydroSafe IoT - Monitoramento de Enchentes com LCD

## 🧠 Descrição

Este projeto simula um sistema de alerta de enchentes utilizando Arduino UNO, sensor ultrassônico HC-SR04, LEDs, buzzer e um display LCD I2C. A solução identifica o nível da água e classifica a situação em três estados: **OK**, **Alerta** e **Perigo**. É uma aplicação da proposta **HydroSafe**, da empresa fictícia *Elevate Consult*, parte da Global Solution 2025.1 da FIAP.

## 🔌 Componentes Utilizados

- 1x Arduino UNO
- 1x Sensor Ultrassônico HC-SR04
- 1x Display LCD I2C (16x2)
- 1x Buzzer ativo
- 3x LEDs (Verde, Amarelo e Vermelho)
- Resistores (220Ω)
- Jumpers e protoboard

## 🧭 Funcionamento

A distância do sensor ao nível da água é convertida para altura de enchente. Com base nessa medida, o sistema:

| Estado        | Distância (cm)    | Ações                                                                 |
|---------------|-------------------|-----------------------------------------------------------------------|
| **OK**        | > 300 cm          | LED verde pisca, LCD mostra "Estado OK" com distância                |
| **Alerta**    | 236 - 300 cm      | LED amarelo pisca, LCD mostra "Estado Alerta" com distância          |
| **PERIGO**    | ≤ 235 cm          | LED vermelho pisca, buzzer toca, LCD mostra "PERIGO" com distância   |

> A distância é ajustada considerando uma profundidade de referência (335 cm) para simular o nível de água acumulada.

## 🎮 Simulação

Simule este projeto no [Tinkercad](https://www.tinkercad.com/things/9lMz4WCONz3-gs-edgecomputing/editel?returnTo=https%3A%2F%2Fwww.tinkercad.com%2Fdashboard%2Fdesigns%2Fcircuits)

## 🎥 Vídeo de Apresentação

Clique para assistir à demonstração completa do funcionamento do sistema:

▶️ **[Assistir no Loom](https://www.loom.com/share/7ef9e8d997144262900828017daf74cb?sid=d8feaeea-1d1c-4e14-b312-70c045b341bb)**
