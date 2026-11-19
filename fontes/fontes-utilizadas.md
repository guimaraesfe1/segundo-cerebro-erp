# Fontes Utilizadas

Este documento registra as fontes de referência do segundo cérebro sobre **utilização de sistemas ERP na gestão empresarial**, com a justificativa de cada escolha e o status de inclusão no NotebookLM.

## Critérios de seleção

As fontes foram escolhidas com base nos seguintes critérios:

- **Origem oficial:** conteúdo publicado diretamente por fabricantes de software (Odoo, SAP, Oracle/NetSuite) ou pelo projeto oficial da ferramenta (PostgreSQL).
- **Relevância:** abordagem dos módulos e processos estudados (estoque, vendas, PDV, compras, financeiro, fiscal e relatórios) e da base técnica de um ERP (banco de dados).
- **Atualização:** materiais mantidos pelos próprios fornecedores.
- **Diversidade:** combinação de solução de código aberto com documentação pública (Odoo), soluções corporativas globais (SAP e Oracle/NetSuite) e documentação técnica de banco de dados (PostgreSQL).

## Legenda de status

| Símbolo | Significado |
|:-------:|-------------|
| ⬜ | Pendente |
| ✅ | Concluído, com evidência em [`../evidencias/fontes/`](../evidencias/fontes/) |
| ⚠️ | Adicionada com ressalvas |

- **Adicionada:** a fonte aparece no painel de fontes do notebook ([`01-fontes-adicionadas.png`](../evidencias/fontes/01-fontes-adicionadas.png)).
- **Verificada:** as citações das respostas foram abertas e conferidas com o conteúdo da fonte.

---

## 1. Odoo Documentation

| Campo | Informação |
|-------|------------|
| **Nome** | Odoo Documentation (versão 20.0) |
| **Link** | https://www.odoo.com/documentation/20.0/ |
| **Tipo de conteúdo** | Documentação técnica e funcional oficial (site) |
| **Assunto abordado** | Funcionamento dos aplicativos do Odoo: inventário, vendas, PDV, compras, contabilidade/financeiro e relatórios |
| **Justificativa** | Documentação pública, detalhada e mantida pelo próprio fabricante, com descrições passo a passo das operações de cada módulo. Ideal para explicar o uso prático de um ERP. |
| **Adicionada no NotebookLM** | ✅ Sim (aparece como "Odoo Documentation — Odo...") |
| **Verificada no NotebookLM** | ⬜ Pendente |
| **Observações** | Foi adicionada a página inicial da documentação. |

## 2. SAP — What is ERP?

| Campo | Informação |
|-------|------------|
| **Nome** | What is ERP? (SAP) |
| **Link** | https://www.sap.com/resources/what-is-erp |
| **Tipo de conteúdo** | Artigo oficial do fabricante (site) |
| **Assunto abordado** | Conceito de ERP, módulos, integração e benefícios de um sistema integrado de gestão |
| **Justificativa** | A SAP é uma das principais fornecedoras de ERP do mundo. O artigo apresenta uma visão conceitual de como o ERP integra os processos de uma empresa. |
| **Adicionada no NotebookLM** | ✅ Sim (aparece como "What is ERP? The Essential G...") |
| **Verificada no NotebookLM** | ⬜ Pendente |
| **Observações** | — |

## 3. Oracle ERP

| Campo | Informação |
|-------|------------|
| **Nome** | Oracle ERP |
| **Link** | https://www.oracle.com/erp/ |
| **Tipo de conteúdo** | Página institucional oficial do fabricante (site) |
| **Assunto abordado** | Conceito de ERP e áreas atendidas (finanças, compras, gestão de projetos, cadeia de suprimentos) |
| **Justificativa** | A Oracle é uma das principais fornecedoras de ERP corporativo do mundo, complementando a visão conceitual da SAP. |
| **Adicionada no NotebookLM** | ✅ Sim (aparece como "Enterprise Resource Planning...") |
| **Verificada no NotebookLM** | ⬜ Pendente |
| **Observações** | — |

## 4. NetSuite — ERP Use Cases

| Campo | Informação |
|-------|------------|
| **Nome** | ERP Use Cases (Oracle NetSuite) |
| **Link** | https://www.netsuite.com/portal/resource/articles/erp/erp-use-cases.shtml |
| **Tipo de conteúdo** | Artigo oficial do fabricante (site) |
| **Assunto abordado** | Casos de uso de ERP em diferentes áreas e setores da empresa |
| **Justificativa** | Conteúdo publicado pela NetSuite (Oracle), fabricante de ERP, com exemplos práticos de aplicação do sistema. |
| **Adicionada no NotebookLM** | ✅ Sim (aparece como "15 Use Cases for Enterprise R...") |
| **Verificada no NotebookLM** | ⬜ Pendente |
| **Observações** | — |

## 5. PostgreSQL Documentation

| Campo | Informação |
|-------|------------|
| **Nome** | PostgreSQL Documentation |
| **Link** | https://www.postgresql.org/docs/ |
| **Tipo de conteúdo** | Documentação técnica oficial (site) |
| **Assunto abordado** | Banco de dados relacional |
| **Justificativa** | A diretriz do especialista inclui banco de dados e modelagem de dados. O PostgreSQL é o banco utilizado pelo Odoo, e sua documentação oficial dá suporte aos aspectos técnicos. |
| **Adicionada no NotebookLM** | ✅ Sim (aparece como "PostgreSQL: Documentation") |
| **Verificada no NotebookLM** | ⬜ Pendente |
| **Observações** | Foi adicionada a página índice da documentação, que contém pouco conteúdo técnico. |

## 6. Canal oficial do Odoo (YouTube)

| Campo | Informação |
|-------|------------|
| **Nome** | Canal oficial do Odoo |
| **Link** | https://www.youtube.com/@Odoo |
| **Tipo de conteúdo** | Vídeos oficiais (tutoriais e demonstrações) |
| **Assunto abordado** | Demonstrações práticas do uso dos módulos do Odoo |
| **Justificativa** | Canal mantido pelo fabricante, com demonstrações visuais que complementam a documentação escrita. |
| **Adicionada no NotebookLM** | ⚠️ Sim, com ressalva (aparece como "Odoo - YouTube") |
| **Verificada no NotebookLM** | ⬜ Pendente |
| **Observações** | Foi adicionado o link do canal, e não de um vídeo específico. O NotebookLM importa transcrições apenas de vídeos individuais, portanto o conteúdo aproveitado desta fonte provavelmente se limita à página do canal. |

---

## Resumo

| # | Fonte | Tipo | Adicionada | Verificada |
|---|-------|------|:----------:|:----------:|
| 1 | [Odoo Documentation](https://www.odoo.com/documentation/20.0/) | Documentação | ✅ | ⬜ |
| 2 | [SAP — What is ERP?](https://www.sap.com/resources/what-is-erp) | Artigo | ✅ | ⬜ |
| 3 | [Oracle ERP](https://www.oracle.com/erp/) | Site institucional | ✅ | ⬜ |
| 4 | [NetSuite — ERP Use Cases](https://www.netsuite.com/portal/resource/articles/erp/erp-use-cases.shtml) | Artigo | ✅ | ⬜ |
| 5 | [PostgreSQL Documentation](https://www.postgresql.org/docs/) | Documentação | ✅ | ⬜ |
| 6 | [Canal oficial do Odoo](https://www.youtube.com/@Odoo) | Vídeos | ⚠️ | ⬜ |

> Evidência das fontes adicionadas: [`../evidencias/fontes/01-fontes-adicionadas.png`](../evidencias/fontes/01-fontes-adicionadas.png).
