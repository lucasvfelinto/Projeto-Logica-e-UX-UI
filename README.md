# Projeto: Sistema Bancário Simples

### Visão Geral do Projeto

O objetivo deste projeto é desenvolver uma aplicação de operações bancárias simples que permita aos operadores realizar ações como criar contas, transferir valores entre contas, exibir informações de contas, remover contas e debitar valores de contas existentes. A aplicação deve ser intuitiva, eficiente e acessível, proporcionando uma boa experiência ao usuário.

## Especificação Detalhada dos Requisitos

### Lógica de Programação

#### **1\. Criação de Contas**

* #### **Entrada de Dados:**

  * #### O usuário deve fornecer:

    * #### Nome completo

    * #### Telefone

    * #### Data de nascimento

* #### **Número da Conta:**

  * #### O número da conta deve ser gerado automaticamente, iniciando em 1 e incrementando para cada nova conta criada.

* #### **Saldo Inicial:**

  * #### Cada conta deve ser criada com um saldo inicial de 1000 reais.

* #### **Estrutura de Dados:**

  * #### Os dados das contas devem ser armazenados em uma matriz com as seguintes colunas:

    * #### Nomes

    * #### Telefone

    * #### Data de Nascimento

    * #### Número da Conta

    * #### Saldo

#### **2\. Inserção de Dados(Criação de Conta)**

* #### **Utilização do Prompt:**

  * #### Todos os dados de entrada devem ser solicitados utilizando a função `prompt`.

  * #### O operador deve inserir:

    * #### Nome completo

    * #### Telefone

    * #### Data de nascimento

* #### **Cálculo Automático:**

  * #### O número da conta deve ser calculado automaticamente com base no número de contas já inseridas.

  * #### O saldo inicial de 1000 reais deve ser atribuído automaticamente a cada nova conta.

#### **3\. Funções a Desenvolver**

* #### **Função Inserir:**

  * #### Descrição: Cria uma nova conta bancária.

  * #### Entradas:

    * #### Nome completo (via `prompt`)

    * #### Telefone (via `prompt`)

    * #### Data de nascimento (via `prompt`)

  * #### Processamento:

    * #### Calcular o número da conta automaticamente.

    * #### Atribuir o saldo inicial de 1000 reais.

    * #### Inserir os dados na matriz de contas.

  * #### Saída: Mensagem de confirmação (via `alert`).

* #### **Função Transferir:**

  * #### Descrição: Realiza uma transferência entre duas contas.

  * #### Entradas:

    * #### Conta de origem (via `prompt`)

    * #### Conta de destino (via `prompt`)

    * #### Valor da transferência (via `prompt`)

  * #### Processamento:

    * #### Verificar se ambas as contas existem.

    * #### Verificar se o saldo da conta de origem é suficiente.

    * #### Subtrair o valor da conta de origem e adicionar à conta de destino.

  * #### Saída: Mensagem de confirmação ou erro (via `alert`).

* #### **Função Exibir:**

  * #### Descrição: Exibe os dados de uma conta específica.

  * #### Entradas:

    * #### Número da conta (via `prompt`)

  * #### Processamento:

    * #### Verificar se a conta existe.

    * #### Recuperar e exibir os dados da conta.

  * #### Saída: Dados da conta (via `alert`).

* #### **Função Remover:**

  * #### Descrição: Remove uma conta bancária.

  * #### Entradas:

    * #### Número da conta (via `prompt`)

  * #### Processamento:

    * #### Verificar se a conta existe.

    * #### Remover a conta da matriz.

  * #### Saída: Mensagem de confirmação ou erro (via `alert`).

* #### **Função Debitar:**

  * #### Descrição: Debita um valor de uma conta.

  * #### Entradas:

    * #### Número da conta (via `prompt`)

    * #### Valor a ser debitado (via `prompt`)

  * #### Processamento:

    * #### Verificar se a conta existe.

    * #### Verificar se o saldo é suficiente.

    * #### Subtrair o valor do saldo da conta.

  * #### Saída: Mensagem de confirmação ou erro (via `alert`).

#### **4\. Tratamento de Erros**

* #### **Condições de Erro:**

  * #### Conta não existente.

  * #### Saldo insuficiente para débito ou transferência.

* #### **Mensagem de Erro:**

  * #### Deve ser exibida uma mensagem de erro apropriada (via `alert`) caso ocorra algum erro durante a execução das funções.

#### **5\. Interface**

* #### **Botões:**

  * #### Cada função deve ser acionada por um botão específico na interface da aplicação.

#### **6\. Desenvolvimento Colaborativo**

* #### **Equipes:**

  * #### O projeto deve ser desenvolvido em trio ou dupla.

* #### **Versionamento:**

  * #### É obrigatório o uso do GitHub para controle de versão e colaboração.



### UX/UI

#### **1\. Protótipo de Alta Fidelidade**

* **Objetivo:**  
  * Criar uma aplicação que permita ao operador realizar operações bancárias de forma intuitiva e eficiente.

#### **2\. Pesquisa de Concorrentes**

* **Análise de Mercado:**  
  * Realizar uma pesquisa sobre concorrentes para identificar as melhores práticas em termos de layout e arquitetura de informação.  
  * Focar em aspectos como facilidade de uso, clareza na apresentação de informações e eficiência nas operações bancárias.

#### **3\. Arquitetura da Informação**

* **Estrutura da Aplicação:**  
  * Tela Inicial:  
    * Botões para cada operação: Inserir Conta, Transferir, Exibir Conta, Remover Conta, Debitar.  
  * Tela de Inserção de Conta:  
    * Campos de entrada: Nome completo, Telefone, Data de nascimento.  
    * Botão de confirmação para criar a conta.  
  * Tela de Transferência:  
    * Campos de entrada: Conta de origem, Conta de destino, Valor da transferência.  
    * Botão de confirmação para realizar a transferência.  
  * Tela de Exibição de Conta:  
    * Campo de entrada: Número da conta.  
    * Botão para exibir os dados da conta.  
  * Tela de Remoção de Conta:  
    * Campo de entrada: Número da conta.  
    * Botão para confirmar a remoção da conta.  
  * Tela de Débito:  
    * Campo de entrada: Número da conta, Valor a ser debitado.  
    * Botão de confirmação para realizar o débito.

#### **4\. Layout e Design**

* **Design Limpo e Intuitivo:**  
  * Utilizar um layout limpo com uma paleta de cores que facilite a leitura e a usabilidade.  
  * Agrupar funcionalidades relacionadas para melhorar a navegação.  
* **Componentes de Interface:**  
  * Utilizar botões grandes e claramente identificáveis para cada operação.  
  * Campos de entrada devem ser suficientemente grandes e bem espaçados para evitar erros de digitação.  
* **Feedback Visual:**  
  * Fornecer feedback visual imediato para cada ação do usuário (ex. mensagens de confirmação, alertas de erro).  
  * Utilizar cores e ícones para indicar estados de sucesso, erro, ou alerta.

#### **5\. Navegação e Usabilidade**

* **Fluxo de Usuário:**  
  * Projetar o fluxo de usuário para que cada operação seja intuitiva e rápida de realizar.  
  * Minimizar o número de cliques necessários para completar uma tarefa.  
* **Acessibilidade:**  
  * Garantir que a aplicação seja acessível para todos os usuários, incluindo aqueles com deficiências visuais ou motoras.  
  * Utilizar etiquetas claras para todos os campos de entrada e botões.  
  * Implementar navegação por teclado e compatibilidade com leitores de tela.

#### **6\. Testes de Usabilidade**

* **Sessões de Teste:**  
  * Conduzir testes de usabilidade com usuários reais para identificar pontos de fricção e áreas de melhoria.  
  * Observar como os usuários interagem com o protótipo e recolher feedback.  
* **Iteração:**  
  * Basear-se no feedback dos testes para iterar e melhorar o design.  
  * Ajustar a arquitetura da informação, layout, e componentes de interface conforme necessário para otimizar a experiência do usuário.

## 

## 

## 

## 

## 

## 

## 

## 

## Divisão dos Requisitos de Lógica para 3 Integrantes do Grupo

### Integrante 1: Criação de Contas e Função Inserir

#### **Responsabilidades:**

* #### **Criação de Contas:**

  * #### Desenvolver a lógica para a criação de contas bancárias.

  * #### Implementar a função para gerar o número da conta de forma incremental, começando do número 1\.

  * #### Garantir que cada nova conta seja criada com um saldo inicial de 1000 reais.

* #### **Função Inserir:**

  * #### Implementar a função `inserir`, que solicita o nome completo, telefone e data de nascimento do usuário.

  * #### Integrar a função de criação de contas com a matriz de dados.

  * #### Utilizar `prompt` para a entrada de dados e `alert` para confirmação.

#### **Entregáveis:**

* #### Função de criação de contas implementada.

* #### Função `inserir` funcionando corretamente e integrada à matriz de dados.

* #### Comentários no código explicando a lógica de criação de contas.

### Integrante 2: Funções de Transferir e Exibir

#### **Responsabilidades:**

* #### **Função Transferir:**

  * #### Desenvolver a função `transferir`, que solicita a conta de origem, a conta de destino e o valor da transferência.

  * #### Implementar verificações para garantir que ambas as contas existam e que o saldo da conta de origem seja suficiente.

  * #### Atualizar os saldos das contas envolvidas na transferência.

  * #### Utilizar `prompt` para a entrada de dados e `alert` para confirmação ou mensagens de erro.

* #### **Função Exibir:**

  * #### **I**mplementar a função `exibir`, que solicita o número da conta e exibe todos os dados da conta cadastrada.

  * #### Verificar se a conta existe antes de exibir os dados.

  * #### Utilizar `prompt` para a entrada de dados e `alert` para exibição dos dados da conta.

#### **Entregáveis:**

* #### Função `transferir` implementada e testada.

* #### Função `exibir` implementada e testada.

* #### Comentários no código explicando a lógica de transferência e exibição de dados.

### Integrante 3: Funções de Remover e Debitar

#### **Responsabilidades:**

* #### **Função Remover:**

  * #### Desenvolver a função `remover`, que solicita o número da conta a ser removida.

  * #### Implementar verificações para garantir que a conta exista antes de removê-la da matriz.

  * #### Atualizar a matriz de dados após a remoção da conta.

  * #### Utilizar `prompt` para a entrada de dados e `alert` para confirmação ou mensagens de erro.

* #### **Função Debitar:**

  * #### Implementar a função `debitar`, que solicita o número da conta e o valor a ser debitado.

  * #### Verificar se a conta existe e se o saldo é suficiente antes de realizar o débito.

  * #### Atualizar o saldo da conta após o débito.

  * #### Utilizar `prompt` para a entrada de dados e `alert` para confirmação ou mensagens de erro.

* #### **Tratamento de Erros:**

  * #### Implementar mensagens de erro apropriadas para casos como conta não existente ou saldo insuficiente.

#### **Entregáveis:**

* #### Função `remover` implementada e testada.

* #### Função `debitar` implementada e testada.

* #### Comentários no código explicando a lógica de remoção e débito.

* #### Tratamento de erros implementado.