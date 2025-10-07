# Calculadora-de-Custos
Trabalho do Sandro Mesquita
# SISTEMA DE GESTÃO DE CUSTOS E AUTONOMIA DE VIAGEM

## Visão Geral do Projeto

Este projeto consiste em uma *Calculadora de Custos e Autonomia de Viagem* desenvolvida em C++. O sistema simula o cálculo do tempo de deslocamento, a quantidade de combustível necessária e o custo total de uma viagem.

O principal diferencial é a aplicação de uma *penalidade de autonomia* caso a velocidade média ultrapasse $100 \text{ km/h}$.

O projeto foi executado sob metodologia de Engenharia de Software, apresentando evidências de gestão (Trello), planejamento visual (Lucidchart) e testes (QA).

---

## Requisitos e Regras de Negócio

O sistema opera com base nas seguintes entradas e na regra de penalidade:

### 1. Entradas Validadas
O sistema exige que os seguintes valores sejam maiores que zero (ou não negativos) para prosseguir:
* *[span_0](start_span)Velocidade Média* (averageSpeed) em $\text{km/h}$[span_0](end_span).
* *[span_1](start_span)Autonomia Original* (vehicleAutonomy) em $\text{km}/\text{l}$[span_1](end_span).
* *[span_2](start_span)Distância* do percurso em $\text{km}$[span_2](end_span).
* *[span_3](start_span)Preço por Litro* de combustível em $\text{R}\$$[span_3](end_span).

### 2. Regra de Penalidade
* *[span_4](start_span)[span_5](start_span)Limite de Velocidade:* $100.0 \text{ km/h}$ (SPEED_LIMIT_FOR_PENALTY)[span_4](end_span)[span_5](end_span).
* *[span_6](start_span)Fator de Redução:* Se a velocidade for maior que o limite[span_6](end_span)[span_7](start_span)[span_8](start_span), a autonomia original do veículo é reduzida por um fator de $0.90$ (AUTONOMY_REDUCTION_FACTOR)[span_7](end_span)[span_8](end_span).

### 3. Fórmulas de Saída
O programa exibe os seguintes resultados:
* *[span_9](start_span)[span_10](start_span)Tempo de Deslocamento:* $\text{Tempo} = \text{Distância} / \text{Velocidade}$ (Convertido para hora(s) e minuto(s))[span_9](end_span)[span_10](end_span).
* *[span_11](start_span)[span_12](start_span)Combustível Necessário:* $\text{Litros} = \text{Distância} / \text{Autonomia Considerada}$[span_11](end_span)[span_12](end_span).
* *[span_13](start_span)[span_14](start_span)Custo Total:* $\text{Custo} = \text{Combustível Necessário} \times \text{Preço por Litro}$[span_13](end_span)[span_14](end_span).

---

## Instalação e Execução

[span_15](start_span)O projeto é um programa de console desenvolvido em C++[span_15](end_span).

### Pré-requisitos
* Um compilador C++ (g++ recomendado).

### Passos de Execução
1.  *Clone o repositório:*
    bash
    git clone [LINK DO SEU REPOSITÓRIO GITHUB AQUI]
    cd calculadora-custos
    
2.  *Compile o código:*
    bash
    g++ main.cpp -o calculadora
    
3.  *Execute e insira os dados:*
    bash
    ./calculadora
    

---

## Organização e Equipe do Projeto

[span_16](start_span)O projeto foi executado pela seguinte equipe[span_16](end_span):

| Membro | Função |
| :--- | :--- |
| *Francisco Antônio Nunes* | [span_17](start_span)Teach Leader[span_17](end_span) |
| *Sibelly Saraiva* | [span_18](start_span)Q.A (Testes)[span_18](end_span) |
| *José Kauã* | [span_19](start_span)Q.A (Testes)[span_19](end_span) |
| *Levi Lima* | [span_20](start_span)Desenvolvedor[span_20](end_span) |
| *Alexandre Mário Soares* | [span_21](start_span)Desenvolvedor[span_21](end_span) |
| *Pedro Henrique Reis* | [span_22](start_span)Desenvolvedor[span_22](end_span) |
| *Ana Carolina Santos* | [span_23](start_span)Documentação[span_23](end_span) |
| *Zacarias da Mata* |  .[span24](start span).Q.A (Testes).(span 24). |

---

## Evidências e Documentação Obrigatória (Entrega AVA)

O link deste README.md no GitHub é o ponto de partida para o professor acessar todas as evidências de gestão e planejamento solicitadas.

| Requisito | Artefato | Link para Acesso Público |
| :--- | :--- | :--- |
| *Gestão do Projeto* | Quadro Trello (Kanban) | **https://trello.com/b/XZdXLumg/calculadora-custos** |
| *Documentação Detalhada* | Relatório de Testes (QA) e Manuais | *https://drive.google.com/drive/folders/13UbOnyw4RiO_hTPTSuC29P_A9eV45OaH?usp=sharing* |

---

## Relatório de Qualidade (QA) - Sumário

A equipe de Q.A. (Sibelly Saraiva, Zacarias da Mata e José Kauã) [span_24](start_span)[span_25](start_span)[span 26](start span]executou testes no OnlineGDB[span_24](end_span)[span_25][span 26](end_span).

* *[span_26](start_span)Objetivo do Teste:* Verificar se o programa calcula corretamente o tempo de viagem, a quantidade de combustível necessária e o custo total, incluindo a redução de autonomia para velocidades acima de $100 \text{ km/h}$[span_26](end_span).
* *[span_27](start_span)Procedimento:* O programa foi executado com entradas válidas em 4 cenários diferentes[span_27](end_span).
* *[span_28](start_span)Conclusão:* Todos os testes foram concluídos com sucesso[span_28](end_span). [span_29](start_span)O programa demonstrou ser confiável e atende aos requisitos propostos[span_29](end_span).
* *[span_30](start_span)Detalhes:* Os resultados detalhados (tabela de cenários) estão na documentação detalhada[span_30](end_span).
