# Capitallab Investment Tool: Simulador de Fundos Imobiliários em Excel (Análise e Automação Financeira)

<img width="952" height="284" alt="Capitallab Investment Tool Banner" src="https://github.com/user-attachments/assets/2ae1fd2a-ea25-4abb-a8bb-d1fa09a4c153" />

## Visão geral do projeto

Este projeto é um simulador de investimentos em FIIs (fundos imobiliários) desenvolvido em excel com foco em decisão baseada em dados e automação de cálculos financeiros. demonstra proficiência na aplicação de fórmulas financeiras reais (valor acumulado, dividend yield, juros compostos) para criar uma ferramenta analítica e intuitiva, pronta para otimizar a tomada de decisão do usuário ao projetar seu patrimônio futuro.

## Habilidades técnicas e analíticas demonstradas

Recrutadores, notem a aplicação prática nas seguintes áreas:

* Modelagem financeira: implementação de fórmulas de juros compostos e projeção de dividendos mensais para simulação de cenários de 0 a 50 anos.
* Análise e visualização de dados: construção de painéis de controle (tabelas e gráficos) em excel para traduzir projeções em informações úteis (ex: curva de crescimento patrimonial).
* Automação e otimização (fácil uso no excel): uso estratégico de recursos como validação de dados e variáveis globais para garantir que o uso seja fácil e a manutenção do modelo, simples.
* Documentação e versionamento: gestão completa do projeto e documentação técnica utilizando o github.

---

## Etapas do desenvolvimento

O projeto foi executado com base em um plano de análise de requisitos e modelagem de dados.

### ETAPA 1: Definição de escopo e estratégia de negócio

O ponto de partida foi a definição dos indicadores chave de desempenho. A ferramenta foi concebida para responder a perguntas críticas que guiam a decisão do investidor:

* Quanto será investido por mês?
* Qual o período de investimento?
* Qual a taxa de rendimento mensal?
* Qual será o valor total acumulado?
* Qual será o valor do dividendo mensal?

A identidade visual (Capitallab) foi criada para estabelecer uma marca forte e profissional, utilizando cores associadas à estabilidade e crescimento no mercado financeiro (verde/branco).

### ETAPA 2: Modelagem de dados e facilidade de uso (simulador de cenários)

Foi iniciada a estruturação do simulador focando na modelagem do crescimento patrimonial (juros compostos).

#### 2.1. Simulação patrimônio x investimento

A tabela e o gráfico de simulação fornecem uma visualização imediata da projeção de patrimônio.

<img width="522" height="379" alt="Tabela de Simulação Patrimônio x Investimento" src="https://github.com/user-attachments/assets/927bef1b-7492-4d10-9607-1378ad282f2e" />

Para otimizar a facilidade de uso, foi utilizada a validação de dados no final da tabela, permitindo que o usuário personalize o horizonte de investimento (0 a 50 anos) sem alterar o modelo central.

#### 2.2. Variáveis globais (configurações iniciais)

Criação da seção de variáveis globais (configurações iniciais). essa centralização de dados de entrada (como salário, taxa de rendimento, aporte mensal) permitiu o refinamento e a correção das fórmulas financeiras, garantindo a precisão dos cálculos e a facilidade de manutenção do modelo.

<img width="511" height="107" alt="Tabela de Configurações Iniciais" src="https://github.com/user-attachments/assets/6659707d-96c7-434e-9495-a1dc86b237b9" />

*Nota: foi adicionada uma sugestão inicial de investimento de 30% da renda mensal como uma funcionalidade de orientação ao usuário.*

#### 2.3. Otimização e estrutura de fórmulas

Para garantir a clareza e a manutenção das fórmulas em todo o modelo, foi implementada a nomeação de intervalos no excel.

* Decisão técnica: ao invés de referências de células estáticas (ex: $A$1), os intervalos de dados críticos (como "salário" ou "taxa_mensal") foram nomeados. isso melhorou a legibilidade, evitou erros de cálculo e facilitou a auditoria do modelo financeiro.

<img width="542" height="422" alt="Nomeação de Intervalos" src="https://github.com/user-attachments/assets/00454d26-b023-409e-9cf3-5fd24abdba50" />

## ETAPA 3: Decisão de alocação e sugestão de perfil de risco

Esta etapa focou em traduzir as necessidades do usuário em uma estratégia de investimento prática, demonstrando raciocínio de negócio.

### 3.1. Análise e recomendação de perfil

Foi desenvolvida uma tabela para avaliação do perfil do investidor (conservador, moderado, agressivo).

* Lógica de negócio: com base no perfil determinado, a tabela define a porcentagem ideal de alocação de capital em diferentes categorias de FIIs (ex: FIIs de tijolo, FIIs de papel). isso transforma o simulador em uma ferramenta de recomendação ativa.

<img width="588" height="512" alt="Tabela de Perfil do Investidor" src="https://github.com/user-attachments/assets/4e2e8c57-92e1-4d6b-b84f-b3562d68bd33" />

### 3.2. Visualização da estratégia de alocação

O gráfico representa visualmente a divisão de fundos que a tabela de perfil de aplicação indicou. essa visualização clara facilita a compreensão da estratégia de alocação de risco e é crucial para a experiência do usuário.

## Conclusão do projeto

O projeto foi concluído resultando no Simulador de Investimentos Capitallab, uma ferramenta que integra modelagem financeira, organização estrutural de dados (nomeação de intervalos) e lógica de recomendação de negócio para auxiliar o usuário na tomada de decisão sobre investimentos em FIIs.

## Próximos passos e evolução

Para o futuro, este projeto pode ser expandido e aprimorado com as seguintes funcionalidades:

* Integração de dados reais: buscar e integrar dados atuais de mercado (como dividend yields e cotações) via api ou web scraping (power query), transformando o simulador em uma ferramenta dinâmica.
* Análise de sensibilidade: adicionar um módulo para simular o impacto de mudanças nas taxas de rendimento e inflação ao longo do tempo.
* Migração para linguagem de programação: planejar a migração do modelo lógico para python ou outra linguagem, visando escalabilidade e o desenvolvimento de uma interface web.
