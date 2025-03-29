# Especificações do Projeto

<span style="color:red">Pré-requisitos: <a href="1-Documentação de Contexto.md"> Documentação de Contexto</a></span>

Este documento apresenta as especificações do projeto IMC Pro, uma plataforma digital para monitoramento do Índice de Massa Corporal e promoção de bem-estar. Utilizamos técnicas como definição de personas, histórias de usuários, modelagem de processos e requisitos funcionais/não funcionais para detalhar a solução.

## Personas

### 1. Ana Carolina Silva
- **Idade:** 32 anos
- **Profissão:** Professora de ensino fundamental
- **Motivação:** Busca melhorar sua saúde após diagnóstico de pré-diabetes
- **Necessidades:** 
  - Monitorar IMC regularmente
  - Receber orientações nutricionais simples
  - Acompanhar progresso de forma visual
  - Alertas sobre mudanças significativas no peso

### 2. Carlos Eduardo Mendes
- **Idade:** 45 anos
- **Profissão:** Executivo de vendas
- **Motivação:** Quer reduzir risco cardiovascular após infarto leve
- **Necessidades:**
  - Acesso rápido à calculadora de IMC
  - Recomendações de exercícios para viagens
  - Histórico de evolução para mostrar ao médico
  - Contato com profissionais de saúde

### 3. Dra. Juliana Almeida
- **Idade:** 38 anos
- **Profissão:** Nutricionista esportiva
- **Motivação:** Busca plataforma para acompanhar pacientes remotamente
- **Necessidades:**
  - Cadastrar planos alimentares personalizados
  - Visualizar progresso dos pacientes
  - Compartilhar materiais educativos
  - Sistema seguro para dados de saúde

### 4. Rodrigo Costa
- **Idade:** 28 anos
- **Profissão:** Personal trainer
- **Motivação:** Quer expandir atendimento online
- **Necessidades:**
  - Criar rotinas de exercícios por objetivos
  - Acompanhar evolução física de clientes
  - Integração com wearables
  - Chat para tirar dúvidas


## Histórias de Usuários

Com base na análise das personas forma identificadas as seguintes histórias de usuários:

|EU COMO... `PERSONA`| QUERO/PRECISO ... `FUNCIONALIDADE` |PARA ... `MOTIVO/VALOR`                 |
|--------------------|------------------------------------|----------------------------------------|
|Usuário do sistema  | Calcular meu IMC          | Acompanhar minha evolução física e avaliar se meu peso está adequado               |
|Usuário do sistema       | Ter um histórico de meus cálculos                |Monitorar meu progresso ao longo do tempo |
|Usuário Comum	   | Receber recomendações personalizadas	  | Melhorar minha saúde com base nas minhas necessidades específicas   |
| Nutricionista	| Compartilhar informações sobre alimentação saudável	| Auxiliar usuários a manterem dieta equilibrada |
| Treinador | 	Recomendar rotinas de exercícios personalizadas	| Garantir que usuários sigam treinos adequados | 
| Administrador | 	Ver estatísticas de usuários	| Monitorar o crescimento e utilização da plataforma| 


## Modelagem do Processo de Negócio 

**Análise da Situação Atual**
Atualmente, pessoas interessadas em monitorar seu IMC utilizam calculadoras básicas disponíveis na internet, sem integração com acompanhamento profissional ou histórico de evolução. Profissionais da saúde não possuem uma plataforma centralizada para acompanhar pacientes.

**Descrição Geral da Proposta**
O IMC Pro oferecerá uma solução integrada com:

Calculadora de IMC avançada

Acompanhamento histórico

Conexão com profissionais de saúde

Conteúdo educativo

Recomendações personalizadas

### Processo 1 - Cálculo e Monitoramento de IMC

Apresente aqui o nome e as oportunidades de melhorias para o processo 1. Em seguida, apresente o modelo do processo 1, descrito no padrão BPMN. 

![Processo 1](img/02-bpmn-proc1.png)

### Processo 2 – Acompanhamento por Profissionais

Apresente aqui o nome e as oportunidades de melhorias para o processo 2. Em seguida, apresente o modelo do processo 2, descrito no padrão BPMN.

![Processo 2](img/02-bpmn-proc2.png)

## Indicadores de Desempenho
Indicadores de Desempenho
Tempo médio para cálculo de IMC (< 5s)

Número de usuários ativos mensais

Taxa de retorno de usuários (≥ 70%)

Número de recomendações enviadas por profissional

Satisfação do usuário (≥ 4/5)

Usar o seguinte modelo: 

![Indicadores de Desempenho](img/02-indic-desemp.png)
Obs.: todas as informações para gerar os indicadores devem estar no diagrama de classe a ser apresentado a posteriori. 

## Requisitos

As tabelas que se seguem apresentam os requisitos funcionais e não funcionais que detalham o escopo do projeto. Para determinar a prioridade de requisitos, aplicar uma técnica de priorização de requisitos e detalhar como a técnica foi aplicada.

### Requisitos Funcionais

| ID | Descrição | Prioridade |
|----|-----------|------------|
| RF-01 | Calculadora de IMC com entrada de peso e altura | Alta |
| RF-02 | Sistema de cadastro/login de usuários | Alta |
| RF-03 | Perfil de usuário com dados pessoais e de saúde | Alta |
| RF-04 | Histórico de cálculos de IMC com gráficos | Média |
| RF-05 | Sistema de alertas para valores críticos de IMC | Alta |
| RF-06 | Módulo para nutricionistas cadastrarem dietas | Alta |
| RF-07 | Módulo para treinadores criarem rotinas de exercícios | Alta |
| RF-08 | Painel administrativo com estatísticas | Média |
| RF-09 | Biblioteca de conteúdos educativos | Baixa |
| RF-10 | Sistema de notificações e lembretes | Média |

### Requisitos não Funcionais

| ID | Descrição | Prioridade |
|----|-----------|------------|
| RNF-01 | Tempo de resposta abaixo de 3 segundos | Alta |
| RNF-02 | Compatibilidade com dispositivos móveis | Alta |
| RNF-03 | Segurança de dados com criptografia | Alta |
| RNF-04 | Acessibilidade (tamanho de fonte ajustável) | Média |
| RNF-05 | Modos claro e escuro | Média |
| RNF-06 | Disponibilidade 24/7 | Alta |

Com base nas Histórias de Usuário, enumere os requisitos da sua solução. Classifique esses requisitos em dois grupos:

- [Requisitos Funcionais
 (RF)](https://pt.wikipedia.org/wiki/Requisito_funcional):
 correspondem a uma funcionalidade que deve estar presente na
  plataforma (ex: cadastro de usuário).
- [Requisitos Não Funcionais
  (RNF)](https://pt.wikipedia.org/wiki/Requisito_n%C3%A3o_funcional):
  correspondem a uma característica técnica, seja de usabilidade,
  desempenho, confiabilidade, segurança ou outro (ex: suporte a
  dispositivos iOS e Android).
Lembre-se que cada requisito deve corresponder à uma e somente uma
característica alvo da sua solução. Além disso, certifique-se de que
todos os aspectos capturados nas Histórias de Usuário foram cobertos.

## Restrições

| ID | Restrição |
|----|-----------|
| 01 | Desenvolvimento em linguagens web modernas |
| 02 | Banco de dados relacional para armazenamento seguro |
| 03 | Conformidade com LGPD para dados de saúde |
| 04 | Integração com APIs de saúde limitadas |

Enumere as restrições à sua solução. Lembre-se de que as restrições geralmente limitam a solução candidata.

> **Links Úteis**:
> - [O que são Requisitos Funcionais e Requisitos Não Funcionais?](https://codificar.com.br/requisitos-funcionais-nao-funcionais/)
> - [O que são requisitos funcionais e requisitos não funcionais?](https://analisederequisitos.com.br/requisitos-funcionais-e-requisitos-nao-funcionais-o-que-sao/)

## Diagrama de Casos de Uso

```mermaid
%%{init: {'theme': 'base', 'themeVariables': { 'primaryColor': '#ffdfd3', 'edgeLabelBackground':'#fff', 'tertiaryColor': '#dcd0ff'}}}%%
useCaseDiagram
    actor Usuário
    actor Nutricionista
    actor Treinador
    actor Administrador
    
    Usuário --> (Calcular IMC)
    Usuário --> (Visualizar histórico)
    Usuário --> (Receber recomendações)
    Usuário --> (Configurar alertas)
    
    Nutricionista --> (Cadastrar dietas)
    Nutricionista --> (Acompanhar pacientes)
    
    Treinador --> (Criar rotinas)
    Treinador --> (Monitorar progresso)

    Administrador --> (Gerenciar usuários)
    Administrador --> (Visualizar estatísticas)
    
    note right of Usuário: Usuários comuns podem\nacessar funcionalidades básicas\nde monitoramento
    note left of Nutricionista: Profissionais de nutrição\ntêm acesso a ferramentas\npara acompanhamento
```

# Matriz de Rastreabilidade

A matriz de rastreabilidade é uma ferramenta usada para facilitar a visualização dos relacionamento entre requisitos e outros artefatos ou objetos, permitindo a rastreabilidade entre os requisitos e os objetivos de negócio. 

A matriz deve contemplar todos os elementos relevantes que fazem parte do sistema, conforme a figura meramente ilustrativa apresentada a seguir.

| ID Requisito | Objetivo | História de Usuário | Caso de Uso |
|--------------|----------|---------------------|-------------|
| RF-01 | Monitoramento básico | Calcular meu IMC | Calcular IMC |
| RF-02 | Segurança e personalização | Criar perfil | Cadastro/Login |
| RF-04 | Acompanhamento contínuo | Ver histórico | Visualizar histórico |
| RF-05 | Prevenção de riscos | Alertas críticos | Configurar alertas |
| RF-06 | Orientação profissional | Dietas personalizadas | Cadastrar dietas |
| RF-10 | Engajamento | Notificações | Sistema de alertas |

![Exemplo de matriz de rastreabilidade](img/02-matriz-rastreabilidade.png)

> **Links Úteis**:
> - [Artigo Engenharia de Software 13 - Rastreabilidade](https://www.devmedia.com.br/artigo-engenharia-de-software-13-rastreabilidade/12822/)
> - [Verificação da rastreabilidade de requisitos usando a integração do IBM Rational RequisitePro e do IBM ClearQuest Test Manager](https://developer.ibm.com/br/tutorials/requirementstraceabilityverificationusingrrpandcctm/)
> - [IBM Engineering Lifecycle Optimization – Publishing](https://www.ibm.com/br-pt/products/engineering-lifecycle-optimization/publishing/)


# Gerenciamento de Projeto

De acordo com o PMBoK v6 as dez áreas que constituem os pilares para gerenciar projetos, e que caracterizam a multidisciplinaridade envolvida, são: Integração, Escopo, Cronograma (Tempo), Custos, Qualidade, Recursos, Comunicações, Riscos, Aquisições, Partes Interessadas. Para desenvolver projetos um profissional deve se preocupar em gerenciar todas essas dez áreas. Elas se complementam e se relacionam, de tal forma que não se deve apenas examinar uma área de forma estanque. É preciso considerar, por exemplo, que as áreas de Escopo, Cronograma e Custos estão muito relacionadas. Assim, se eu amplio o escopo de um projeto eu posso afetar seu cronograma e seus custos.

## Gerenciamento de Tempo

Com diagramas bem organizados que permitem gerenciar o tempo nos projetos, o gerente de projetos agenda e coordena tarefas dentro de um projeto para estimar o tempo necessário de conclusão.

![Diagrama de rede simplificado notação francesa (método francês)](img/02-diagrama-rede-simplificado.png)

O gráfico de Gantt ou diagrama de Gantt também é uma ferramenta visual utilizada para controlar e gerenciar o cronograma de atividades de um projeto. Com ele, é possível listar tudo que precisa ser feito para colocar o projeto em prática, dividir em atividades e estimar o tempo necessário para executá-las.

![Gráfico de Gantt](img/02-grafico-gantt.png)

## Gerenciamento de Equipe

| Nome | Função | Responsabilidades |
|------|--------|-------------------|
| Arthur Messeder Jacques | Dev Front-end |  |
| Hideki Yukinory Pacheco Ishi | Dev Back-end |  |
| Johnata de Souza do Amparo | DB Specialist |  |
| Matheus Henrique Pereira Cruz | UX/UI Designer |  |
| Sara Christine Mendoza | QA Engineer | |

![Simple Project Timeline](img/02-project-timeline.png)

## Gestão de Orçamento

| Item | Custo Estimado (R$) |
|------|---------------------|
| Desenvolvimento | 45.000 |
| Infraestrutura | 12.000 |
| Design/UX | 8.000 |
| Testes | 6.000 |
| Contingência | 5.000 |
| **Total** | **76.000** |
