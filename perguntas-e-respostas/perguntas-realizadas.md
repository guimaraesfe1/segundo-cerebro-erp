# Perguntas Realizadas

Roteiro de testes para validar o funcionamento do segundo cérebro no NotebookLM.

## Instruções de preenchimento

1. Faça cada pergunta no chat do notebook **após** aplicar a [diretriz do especialista](../configuracao/diretriz-especialista.md).
2. Copie a resposta **exatamente como foi gerada** pelo NotebookLM.
3. Clique em cada citação e anote a fonte e o trecho correspondente.
4. Salve capturas de tela da pergunta, da resposta e das citações em [`../evidencias/respostas/`](../evidencias/respostas/).
5. Registre suas observações e aprendizados.

> **Importante:** não preencha os campos com conteúdo hipotético. Registre apenas o que foi efetivamente obtido nos testes.
>
> As respostas abaixo foram copiadas do chat do NotebookLM. Os números entre colchetes (ex.: `[1]`) são as citações exibidas pela ferramenta; ao copiar o texto, o NotebookLM não inclui o nome da fonte correspondente, por isso a identificação de cada citação está pendente.

## Resumo dos testes

| # | Pergunta | Data do teste | Citações verificadas | Evidência |
|---|----------|:-------------:|:--------------------:|:---------:|
| 1 | O que é um ERP e como ele integra os diferentes setores de uma empresa? | 18/11/2026 | ⬜ | ⬜ |
| 2 | Explique passo a passo como funciona uma venda em um ERP, desde o registro no PDV até a atualização do estoque e do financeiro. | 18/11/2026 | ⬜ | ⬜ |
| 3 | Como funciona o controle de estoque em um ERP e quais são os principais cuidados para evitar divergências? | 18/11/2026 | ⬜ | ⬜ |
| Extra | Como construir um ERP para supermercados? Qual design de sistema usar? Qual arquitetura? | 18/11/2026 | ⬜ | ⬜ |

---

## Pergunta 1

### Pergunta

> O que é um ERP e como ele integra os diferentes setores de uma empresa?

**Data do teste:** 18/11/2026

### Resposta obtida

<details>
<summary>Clique para expandir a resposta completa</summary>

Um **ERP** (*Enterprise Resource Planning* ou Planejamento de Recursos Empresariais) é um sistema de software composto por um conjunto de módulos integrados projetados para automatizar e gerenciar os processos fundamentais de uma empresa[1]. Didaticamente, pode-se entender o ERP como o **sistema nervoso central** de uma organização: assim como o corpo humano possui órgãos que operam interligados, uma empresa possui diferentes departamentos (como Finanças, Vendas, Estoque, Compras e Recursos Humanos) que precisam funcionar de forma harmoniosa[4][5].

#### Como o ERP Integra os Diferentes Setores

Em empresas que operam sem um ERP, cada setor costuma utilizar suas próprias ferramentas isoladas ou planilhas (os chamados **silos de dados**)[6]. Isso gera duplicidade de digitação, divergência de informações e falta de visibilidade para a diretoria[6].

O ERP resolve essa fragmentação através de dois pilares fundamentais:

1. **Banco de Dados Único (Centralizado)**: Todos os módulos do software conectam-se a uma mesma base de dados[1]. Quando uma informação é registrada por um departamento, ela é gravada nesse banco central e fica imediatamente disponível para os demais setores[6].
2. **Fonte Única da Verdade (*Single Source of Truth*)**: Como todos os setores compartilham os mesmos dados, elimina-se o conflito de informações (como o setor de vendas visualizar um saldo de estoque diferente do almoxarifado)[2].

#### Passo a Passo: Um Processo Integrado na Prática

Para ilustrar como essa integração ocorre no dia a dia operacional, vejamos o fluxo de um processo de negócio (de **Vendas a Finanças/Suprimentos**):

* **Passo 1 — Registro da Venda (Módulo de Vendas/E-commerce/PDV)**: O vendedor ou o cliente final realiza um pedido[13]. A transação é gravada no sistema.
* **Passo 2 — Atualização de Estoque (Módulo de Logística/SCM)**: Automaticamente, o ERP abate o produto vendido do saldo de estoque, gerando a ordem de separação e expedição sem necessidade de contagens manuais ou comunicação via planilha[10].
* **Passo 3 — Gatilho de Reabastecimento (Módulo de Compras/Procurement)**: Caso o estoque desse item atinja o limite mínimo de segurança, o módulo de Compras é alertado para emitir um pedido de cotação ou compra junto ao fornecedor[12].
* **Passo 4 — Faturamento e Contabilidade (Módulo Financeiro)**: Simultaneamente ao pedido de venda, o módulo de Finanças gera a nota fiscal, registra o lançamento no **Contas a Receber** e atualiza o livro diário contábil[1].
* **Passo 5 — Indicadores e Gestão (Módulo de Relatórios/BI)**: Os executivos conseguem visualizar instantaneamente a receita gerada, a margem de lucro e o impacto no fluxo de caixa por meio de relatórios consolidados em tempo real[11].

#### Principais Benefícios da Integração

* **Efeito Multiplicador**: Ao cruzar dados de módulos distintos (como conectar o histórico do CRM às vendas do E-commerce ou dados de RH ao desempenho da cadeia de suprimentos), a empresa obtém insights estratégicos que superam a soma das partes isoladas[14].
* **Otimização de TI e Produtividade**: Reduz-se drasticamente o esforço manual de reentradas de dados, minimizando erros operacionais e economizando tempo de equipe[6].
* **Tomada de Decisão Ágil**: Com dashboards padronizados e métricas atualizadas em tempo real, a liderança identifica gargalos e novas oportunidades com rapidez[11].

📊 *Podemos explorar em mais detalhes a arquitetura de banco de dados ideal para suportar essa integração ou analisar como estruturar os módulos de um setor específico (como varejo/supermercados).*

</details>

### Fontes citadas pelo NotebookLM

| Nº da citação | Fonte | Trecho citado |
|:-------------:|-------|---------------|
| [1], [2], [4], [5], [6], [10], [11], [12], [13], [14] | _a identificar (clicar na citação no NotebookLM)_ | _a identificar_ |

### Observações e aprendizados

- A resposta definiu ERP, explicou a integração pelo **banco de dados único** e pela **fonte única da verdade** e apresentou um fluxo passo a passo entre módulos (vendas → estoque → compras → financeiro → relatórios).
- Seguiu a diretriz: linguagem didática (analogia com o sistema nervoso central), passo a passo e citações na maior parte das afirmações.
- A frase "A transação é gravada no sistema" (Passo 1) não possui citação própria.
- _Complementar após a verificação das citações._

**Evidência:** _pendente (salvar em `../evidencias/respostas/`)_

---

## Pergunta 2

### Pergunta

> Explique passo a passo como funciona uma venda em um ERP, desde o registro no PDV até a atualização do estoque e do financeiro.

**Data do teste:** 18/11/2026

### Resposta obtida

<details>
<summary>Clique para expandir a resposta completa</summary>

O funcionamento de uma venda dentro de um **ERP** (*Enterprise Resource Planning*) exemplifica como o sistema atua como o **sistema nervoso central** de uma empresa, eliminando silos de dados e integrando processos em tempo real[1][2]. Quando uma transação ocorre no Ponto de Venda (PDV/POS), o ERP executa um fluxo transacional automático que conecta a frente de caixa ao almoxarifado e à contabilidade por meio de uma **base de dados centralizada**[1].

Abaixo está o detalhamento passo a passo desse fluxo, do registro inicial aos impactos financeiros e estratégicos.

#### Passo a Passo da Venda no ERP

##### 1. Registro e Captura da Venda no PDV (Módulo de Vendas/POS)

* **Ação Operacional**: O operador de caixa registra os produtos leitor de código de barras ou seleção manual na interface do PDV[5][6]. O sistema recupera a tabela de preços vigente, aplica eventuais descontos cadastrados e calcula os tributos pertinentes.
* **Geração do Pedido**: Ao confirmar a forma de pagamento (dinheiro, cartão, PIX), o módulo de vendas gera a transação e autoriza a emissão do documento fiscal ou recibo[7][8].
* **Visão Técnica/Dados**: O banco de dados (como PostgreSQL) grava os registros da venda em estruturas relacionais (por exemplo, tabelas `sales_order` e `sales_order_line`), atribuindo um identificador único de transação, dados da filial, data/hora e valores.

##### 2. Baixa Automatizada no Módulo de Estoque (Inventory/SCM)

* **Movimentação Física e Lógica**: Assim que o pagamento é validado, o módulo de inventário recebe a notificação da venda sem necessidade de intervenção humana[3][9]. O ERP abate instantaneamente as quantidades dos itens vendidos do saldo de estoque disponível[9][10].
* **Gatilhos de Reabastecimento**: Caso a quantidade restante do produto atinja o **estoque mínimo de segurança**, o módulo de compras é alertado automaticamente para gerar uma solicitação de cotação ou emissão de Pedido de Compra (PO) ao fornecedor[9][10].
* **Visão Técnica/Integridade**: A atualização de estoque é executada dentro de uma **transação atômica (ACID)** no banco de dados. Isso previne o risco de *race conditions* (quando dois PDVs tentam vender o mesmo item simultaneamente sem que haja saldo suficiente).

##### 3. Integração Contábil e Registro Financeiro (Financial Management)

* **Contas a Receber e Fluxo de Caixa**: O valor pago pelo cliente é direcionado ao módulo financeiro, registrando a entrada no **Contas a Receber** (AR — *Accounts Receivable*) e na conta de caixa/banco[8].
* **Contabilização e CMV**: Simultaneamente, o sistema atualiza o **Livro Razão** (*General Ledger*), contabilizando a receita bruta, os impostos recolhidos e o Custos das Mercadorias Vendidas (CMV), garantindo o fechamento contábil e a reconciliação contínua[8].

##### 4. Atualização de Indicadores e Business Intelligence (BI)

* **Visibilidade em Tempo Real**: Os dados da venda são consolidados imediatamente nos dashboards gerenciais da liderança[8][13].
* **Análise de Desempenho**: O cruzamento de dados permite acompanhar métricas como margem de lucro por produto, horário de maior movimento, taxa de conversão por caixa e impacto instantâneo no fluxo de caixa[8].

#### Resumo da Integração de Dados

| Etapa | Módulo Envolvido | Ação Principal | Resultado no ERP |
|-------|------------------|----------------|------------------|
| **1. Venda** | PDV / Vendas | Captura de itens e pagamento[5][6] | Emissão da nota e registro do pedido[7][8] |
| **2. Estoque** | Gestão de Estoque / SCM | Débito da quantidade vendida[9][10] | Saldo atualizado e alerta de recompra[9][10] |
| **3. Financeiro** | Finanças / Contabilidade | Lançamento em Contas a Receber e Razão[8] | Reconciliação bancária e apuração do CMV[8] |
| **4. Gestão** | BI / Relatórios | Consolidação de métricas[1][15] | Dashboards executivos em tempo real[8][13] |

*(Nota: Embora as fontes cubram a arquitetura conceitual e os fluxos de integração entre módulos de ERP, especificidades de comunicação de hardware local de impressoras térmicas ou bibliotecas fiscais locais de cada país não estão detalhadas no material).*

📊 Se quiser aprofundar a parte de desenvolvimento, podemos modelar o esquema de tabelas (diagrama ER) no banco de dados para suportar essa transação de venda e estoque.

</details>

### Fontes citadas pelo NotebookLM

| Nº da citação | Fonte | Trecho citado |
|:-------------:|-------|---------------|
| [1], [2], [3], [5], [6], [7], [8], [9], [10], [13], [15] | _a identificar (clicar na citação no NotebookLM)_ | _a identificar_ |

### Observações e aprendizados

- A resposta cobriu o fluxo pedido (PDV → estoque → financeiro) e foi além, incluindo compras (reabastecimento) e relatórios/BI, o que demonstra o impacto de uma venda em vários módulos.
- Apresentou uma tabela-resumo da integração e uma nota informando o que **não** está coberto pelas fontes (impressoras térmicas e bibliotecas fiscais locais), em linha com a regra de informar lacunas.
- **Trechos sem citação:** a "Visão Técnica/Dados" (tabelas `sales_order` e `sales_order_line`, PostgreSQL), a "Visão Técnica/Integridade" (transação ACID, *race conditions*) e a frase sobre tabela de preços, descontos e tributos. Esses trechos parecem vir do conhecimento geral do modelo, possivelmente estimulado pela regra 6 da diretriz (exemplos técnicos), e devem ser lidos com cautela.
- A emissão de nota fiscal aparece de forma genérica, sem particularidades do Brasil (ex.: NF-e/NFC-e), o que é coerente com a ausência de fontes nacionais (TOTVS) no notebook.
- _Complementar após a verificação das citações._

**Evidência:** _pendente (salvar em `../evidencias/respostas/`)_

---

## Pergunta 3

### Pergunta

> Como funciona o controle de estoque em um ERP e quais são os principais cuidados para evitar divergências?

**Data do teste:** 18/11/2026

### Resposta obtida

<details>
<summary>Clique para expandir a resposta completa</summary>

O **controle de estoque em um ERP** atua como a ponte entre as operações físicas do almoxarifado/loja e o planejamento financeiro e de compras da empresa[1]. Em vez de depender de contagens manuais esporádicas gravadas em planilhas isoladas — o que frequentemente gera furos de estoque e atrasos na separação de pedidos —, o ERP centraliza todas as movimentações em tempo real em um único banco de dados[1].

#### Como Funciona o Controle de Estoque no ERP (Passo a Passo)

O ciclo de vida das mercadorias dentro do ERP é estruturado em etapas integradas aos demais módulos da empresa:

##### 1. Recebimento e Entrada de Mercadorias (*Inbound*)

* **Conferência e Arrumação**: Ao receber produtos de fornecedores, o ERP permite registrar a entrada em fluxos de uma, duas ou três etapas (como recebimento, conferência e estocagem)[5].
* **Automação de Entrada**: A recepção é validada por meio de leitores de **código de barras** ou **RFID**, garantindo que as quantidades e códigos correspondam exatamente ao Pedido de Compra (*PO*)[5][6].
* **Regras de Endereçamento (*Putaway Rules*)**: O ERP indica automaticamente em qual localização física ou prateleira do armazém o item deve ser guardado[5].

##### 2. Rastreabilidade e Movimentação Interna

* **Identificação Refinada**: O sistema controla os produtos utilizando **números de lote**, **números de série** e **datas de validade**[5].
* **Conversão de Unidades de Medida**: O módulo gerencia a conversão de unidades (por exemplo, comprou em caixa/fardo com 12 unidades e vende em unidade individual)[5].
* **Estratégias de Saída (*Removal Strategies*)**: Na separação de itens, o ERP orienta a retirada com base em regras logísticas:
  * **FEFO** (*First Expired, First Out*): O item com a data de vencimento mais próxima sai primeiro[5].
  * **FIFO** (*First In, First Out*): O item mais antigo no estoque é priorizado para saída[5].

##### 3. Baixa Automática em Vendas (*Outbound / Fulfillment*)

* **Integração com Canais de Venda**: Quando uma venda é realizada no PDV ou no E-commerce, o ERP realiza a baixa instantânea no saldo de estoque disponível[2].
* **Localização Exata para Separação**: O sistema informa aos operadores do armazém a localização precisa de cada produto, otimizando o tempo de separação e expedição[1][2].

##### 4. Reabastecimento Automático (*Replenishment*)

* **Regras de Reposição (*Reordering Rules*)**: O ERP monitora os níveis mínimos de segurança[2][5]. Se o saldo físico ou projetado atinge o ponto de pedido, o sistema aciona regras de reposição automática (*Just-in-Time* ou *MTO - Make to Order*), gerando requisições automáticas para o módulo de Compras[2][5].

#### Principais Cuidados para Evitar Divergências (Estoque Físico vs. Lógico)

Divergências acontecem quando a quantidade real na prateleira não bate com a quantidade registrada no sistema. Para evitar essas falhas, um ERP oferece ferramentas e rotinas essenciais:

1. **Adotar Contagens Cíclicas (*Cycle Counts*)**:
   * *O Cuidado*: Não espere pelo inventário geral no fim do ano[1]. O ERP permite agendar contagens cíclicas contínuas por categorias ou setores[5][8]. Pequenas auditorias diárias ou semanais identificam desvios rapidamente sem parar a operação[5][8].
2. **Eliminar a Digitação Manual com Códigos de Barras / RFID**:
   * *O Cuidado*: Erros de digitação no recebimento ou na separação são as maiores fontes de furos no estoque. O uso de leitores de código de barras e coletores RFID em todas as movimentações (ajustes, transferências e baixas) garante precisão dos dados digitais[5][6].
3. **Registro Rígido de Avarias e Perdas (*Scrap Inventory*)**:
   * *O Cuidado*: Produtos quebrados, danificados ou vencidos devem ser lançados imediatamente na rotina de *Scrap* (descarte/avaria)[5]. Se o operador apenas descartar o item fisicamente sem registrar no ERP, o saldo lógico permanecerá incorreto[5].
4. **Controle Estrito de Validade e Lotes**:
   * *O Cuidado*: No setor alimentício ou farmacêutico, produtos que vencem na prateleira geram prejuízo direto. Configurar alertas de expiração (*expiration dates*) e forçar a regra FEFO garante a rotatividade correta do estoque[5].
5. **Centralização e Eliminação de Silos de Dados**:
   * *O Cuidado*: Evitar a coexistência de planilhas paralelas fora do ERP[1]. Quando todos os setores compartilham o mesmo banco de dados centralizado, o saldo é atualizado de forma síncrona e sem duplicidade[4].

#### Exemplo Prático Empresarial

Imagine uma **distribuidora de produtos alimentícios**:

1. **Recebimento**: Chega uma carga de laticínios. O conferente lê o código de barras da caixa via coletor de dados[5][6]. O ERP valida o lote e a data de validade[5], registrando a entrada e sugerindo a armazenagem na câmara fria (regra de *putaway*)[5].
2. **Venda e Separação**: Ao emitir um pedido de venda no sistema, o ERP direciona a equipe de separação para o lote com vencimento mais próximo (regra FEFO)[5].
3. **Controle de Furos**: Durante uma contagem cíclica semanal[5][8], descobre-se que um iogurte vazou. O operador faz o lançamento de *scrap* (avaria) no sistema[5], ajustando o estoque lógico instantaneamente[5] e disparando um alerta de compra caso atinja o estoque mínimo[2][5].

📊 Podemos modelar o esquema de tabelas (ex: `product`, `stock_location`, `stock_move` e `inventory_adjustment`) no banco de dados PostgreSQL para suportar esse fluxo de controle de estoque. Quer ver essa estrutura técnica?

</details>

### Fontes citadas pelo NotebookLM

| Nº da citação | Fonte | Trecho citado |
|:-------------:|-------|---------------|
| [1], [2], [4], [5], [6], [8] | _a identificar (clicar na citação no NotebookLM)_ | _a identificar_ |

### Observações e aprendizados

- Foi a resposta mais detalhada e prática: cobriu entrada, rastreabilidade (lote, série, validade), estratégias de saída (FEFO/FIFO), baixa automática, reposição e cinco cuidados contra divergências, com um exemplo de distribuidora de alimentos.
- A citação [5] sustenta a maior parte do conteúdo operacional. Os termos usados (*Putaway Rules*, *Removal Strategies*, *Reordering Rules*, *Scrap*) indicam que ela provavelmente vem da documentação do Odoo — **confirmar ao abrir a citação**.
- Mostrou o impacto entre módulos (estoque → compras via reposição; venda → baixa no estoque).
- A afirmação "Erros de digitação [...] são as maiores fontes de furos no estoque" não possui citação.
- _Complementar após a verificação das citações._

**Evidência:** _pendente (salvar em `../evidencias/respostas/`)_

---

## Pergunta extra (fora do roteiro)

### Pergunta

> Como construir um ERP para supermercados? qual design de sistema usar? qual arquitetura?

**Data do teste:** 18/11/2026

### Resposta obtida

Sua nota salva indica apenas a intenção de **"Construir um ERP"**[1], mas **suas fontes não contêm informações detalhadas sobre arquitetura, design de sistemas ou requisitos específicos para um ERP de supermercados**.

Se quiser, posso realizar uma **pesquisa na web** sobre padrões de arquitetura corporativa, módulos essenciais e design de sistemas para ERPs do setor supermercadista. Gostaria que eu fizesse essa pesquisa?

### Fontes citadas pelo NotebookLM

| Nº da citação | Fonte | Trecho citado |
|:-------------:|-------|---------------|
| [1] | Nota salva no notebook ("Meu Segundo Cérebro...") — _confirmar_ | "Construir um ERP" |

### Observações e aprendizados

- **Teste de comportamento bem-sucedido:** o NotebookLM informou claramente que as fontes não continham a informação, em vez de inventar uma resposta, cumprindo as regras 7 e 8 da diretriz.
- A resposta demonstra a limitação do segundo cérebro: ele só responde com segurança sobre o que está nas fontes. Para abordar arquitetura de software de um ERP, seria necessário adicionar fontes específicas sobre o tema.

**Evidência:** _pendente (salvar em `../evidencias/respostas/`)_

---

## Conclusões gerais

- As três perguntas do roteiro foram respondidas com estrutura didática, passo a passo e exemplos práticos, conforme a diretriz.
- As respostas evidenciaram a **integração entre módulos**, tema central do projeto.
- A pergunta extra comprovou que o assistente **reconhece quando as fontes não cobrem um assunto**.
- **Ponto de atenção:** alguns trechos técnicos (modelagem de tabelas, transações ACID) e algumas afirmações gerais aparecem sem citação. Eles devem ser considerados conhecimento complementar do modelo, não informação comprovada pelas fontes.
- _Pendente: verificar a fonte de cada citação e salvar as evidências._
