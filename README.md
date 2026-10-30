# Estacao-Solarimetrica-Angola
Projeto de engenharia para implementação de uma estação solarimétrica no Cunene, Angola, destinada à recolha de dados solares e meteorológicos para dimensionamento de sistemas fotovoltaicos.

# Estação Solarimétrica - Cunene, Angola

**Especificação técnica e lista de materiais para implementação**

## 1. Visão geral

Este repositório reúne a documentação técnica do projeto de desenvolvimento e implementação de uma estação solarimétrica na província do Cunene, Angola.

A estação tem como finalidade recolher, armazenar e disponibilizar dados de irradiância solar e variáveis meteorológicas relevantes para apoiar o dimensionamento, a simulação e a avaliação de sistemas fotovoltaicos na região.

O projeto contempla a integração da instrumentação solarimétrica, sensores meteorológicos, sistema de aquisição de dados, armazenamento local, telecomunicações e infraestrutura de armazenamento e processamento na nuvem AWS.

## 2. Objetivos do projeto

- Medir a irradiância global horizontal (GHI) e a irradiância difusa horizontal (DHI).
- Medir a irradiância no plano dos módulos fotovoltaicos (POA) através de uma célula de referência.
- Monitorizar variáveis meteorológicas relevantes para a caracterização do recurso solar e o dimensionamento FV.
- Adquirir e armazenar os dados localmente.
- Transmitir periodicamente os dados para a nuvem AWS, com armazenamento no Amazon S3.
- Permitir a monitorização remota do estado operacional da estação.
- Disponibilizar dados estruturados para apoiar projetos de sistemas fotovoltaicos.

## 3. Arquitetura geral

A solução está organizada nos seguintes subsistemas:

1. **Instrumentação solarimétrica:** piranómetros para GHI e DHI e célula de referência para POA.
2. **Instrumentação meteorológica:** sensores de temperatura ambiente, humidade relativa e velocidade do vento.
3. **Aquisição e armazenamento local:** microcontrolador, computador de borda, interfaces de comunicação e armazenamento.
4. **Telecomunicações:** transmissão de dados através de LoRa ponto a ponto ou comunicação celular GSM/LTE.
5. **Gateway:** receção dos dados LoRa e encaminhamento para a Internet, quando utilizada essa alternativa.
6. **Infraestrutura AWS:** armazenamento no Amazon S3, processamento e monitorização remota.

## 4. Alternativas de telecomunicações

O projeto contempla duas alternativas:

- **Opção A - LoRa:** comunicação ponto a ponto entre a estação e um gateway remoto, considerando uma distância de referência de até 10 km.
- **Opção B - GSM/LTE:** comunicação celular diretamente a partir da estação para a infraestrutura AWS.

A seleção definitiva dependerá da avaliação técnica do enlace, da cobertura disponível, da compatibilidade dos equipamentos e dos custos de implementação.

## 5. Documentação

A documentação deste repositório inclui:

- Especificação técnica da estação solarimétrica.
- Lista de materiais (BOM).
- Referências comerciais e datasheets dos equipamentos.
- Arquitetura dos subsistemas.
- Diagramas e esquemas de integração.
- Requisitos de instalação e implementação.
- Documentação de telecomunicações e integração com a AWS.

## 6. Princípios de engenharia

O desenvolvimento segue uma abordagem de engenharia prática, orientada à implementação real.

As decisões técnicas deverão considerar:

- Disponibilidade comercial dos equipamentos.
- Compatibilidade entre componentes.
- Pesquisa de fabricantes e fornecedores.
- Custos de aquisição, transporte e instalação.
- Custos de operação e manutenção.
- Fiabilidade, segurança e facilidade de reparação.
- Cumprimento dos requisitos técnicos e normativos aplicáveis.

A prioridade é implementar uma solução funcional, economicamente viável e capaz de produzir dados fiáveis para o dimensionamento de sistemas fotovoltaicos.

## 7. Localização

**Província:** Cunene
**País:** Angola

## 8. Estado do projeto

Em fase de desenvolvimento técnico e preparação para implementação.

A especificação e a lista de materiais deverão ser atualizadas à medida que os equipamentos forem confirmados, adquiridos, integrados e testados.

---

**Projeto:** Estação Solarimétrica - Cunene, Angola
**Documento principal:** Especificação Técnica e Lista de Materiais para Implementação
