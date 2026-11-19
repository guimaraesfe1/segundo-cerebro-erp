# Segundo Cérebro com IA — ERP

> Assistente inteligente especializado em **utilização de sistemas ERP na gestão empresarial**, construído com o Google NotebookLM a partir de fontes confiáveis.

![Status](https://img.shields.io/badge/status-em%20andamento-yellow)
![Ferramenta](https://img.shields.io/badge/ferramenta-Google%20NotebookLM-blue)
![Idioma](https://img.shields.io/badge/idioma-pt--BR-green)

---

## Sumário

1. [Descrição do projeto](#1-descrição-do-projeto)
2. [Objetivo do segundo cérebro](#2-objetivo-do-segundo-cérebro)
3. [Problema que o projeto busca resolver](#3-problema-que-o-projeto-busca-resolver)
4. [Ferramenta utilizada](#4-ferramenta-utilizada)
5. [Assuntos estudados](#5-assuntos-estudados)
6. [Fontes utilizadas](#6-fontes-utilizadas)
7. [Diretriz de comportamento da IA](#7-diretriz-de-comportamento-da-ia)
8. [Perguntas realizadas e resultados](#8-perguntas-realizadas-e-resultados)
9. [Materiais gerados](#9-materiais-gerados)
10. [Evidências do funcionamento](#10-evidências-do-funcionamento)
11. [Notebook compartilhado](#11-notebook-compartilhado)
12. [Tecnologias e ferramentas](#12-tecnologias-e-ferramentas)
13. [Estrutura de diretórios](#13-estrutura-de-diretórios)
14. [Como reproduzir o projeto](#14-como-reproduzir-o-projeto)
15. [Checklist de conclusão](#15-checklist-de-conclusão)

---

## 1. Descrição do projeto

O **segundo-cerebro-erp** documenta a criação de um "segundo cérebro" com Inteligência Artificial: um notebook no Google NotebookLM alimentado com fontes oficiais de fornecedores e plataformas de ERP, configurado para atuar como especialista no tema.

Este repositório reúne a configuração do assistente, as fontes utilizadas, o roteiro de perguntas de teste, os materiais produzidos e as evidências do funcionamento.

## 2. Objetivo do segundo cérebro

Criar um assistente inteligente especializado em sistemas ERP, capaz de explicar funcionalidades, módulos e processos empresariais, sempre embasando suas respostas em fontes confiáveis e citáveis.

Detalhamento: [`configuracao/objetivo.md`](configuracao/objetivo.md).

## 3. Problema que o projeto busca resolver

Estudantes e profissionais iniciantes costumam ter dificuldade para entender um ERP como um sistema **integrado**: cada módulo (estoque, vendas, compras, financeiro, fiscal) costuma ser estudado de forma isolada, e o impacto de uma operação nos demais setores nem sempre fica claro. Além disso, conteúdos genéricos encontrados na internet nem sempre são confiáveis.

O segundo cérebro busca resolver esse problema oferecendo:

- Respostas centralizadas em um único assistente.
- Explicações baseadas em documentação oficial, com citações verificáveis.
- Foco prático, com operações explicadas passo a passo.
- Ênfase na integração entre os módulos.

## 4. Ferramenta utilizada

| Item | Descrição |
|------|-----------|
| **Ferramenta** | [Google NotebookLM](https://notebooklm.google.com/) |
| **Modelo de IA** | Gemini (Google) |
| **Recursos utilizados** | Upload de fontes, chat com citações, instruções personalizadas, geração de mapa mental e materiais de estudo |

O NotebookLM foi escolhido por responder com base **nas fontes adicionadas pelo usuário** e por exibir citações que permitem conferir a origem de cada informação.

## 5. Assuntos estudados

- Fundamentos de sistemas ERP.
- Gestão de estoque e produtos.
- Vendas e PDV (Ponto de Venda).
- Compras e fornecedores.
- Gestão financeira.
- Emissão de notas fiscais.
- Relatórios gerenciais.
- Integração entre os módulos.

## 6. Fontes utilizadas

| # | Fonte | Tipo | Adicionada | Verificada |
|---|-------|------|:----------:|:----------:|
| 1 | [Odoo Documentation](https://www.odoo.com/documentation/20.0/) | Documentação técnica oficial | ✅ | ⬜ |
| 2 | [SAP — What is ERP?](https://www.sap.com/resources/what-is-erp) | Artigo do fabricante | ✅ | ⬜ |
| 3 | [Oracle ERP](https://www.oracle.com/erp/) | Página institucional do fabricante | ✅ | ⬜ |
| 4 | [NetSuite — ERP Use Cases](https://www.netsuite.com/portal/resource/articles/erp/erp-use-cases.shtml) | Artigo do fabricante | ✅ | ⬜ |
| 5 | [PostgreSQL Documentation](https://www.postgresql.org/docs/) | Documentação técnica oficial | ✅ | ⬜ |
| 6 | [Canal oficial do Odoo](https://www.youtube.com/@Odoo) | Vídeos oficiais (YouTube) | ⚠️ | ⬜ |

**Justificativa de confiabilidade:** todas as fontes são **oficiais**, publicadas pelos próprios fabricantes de software (Odoo, SAP, Oracle/NetSuite) ou pelo projeto oficial do PostgreSQL, o que reduz o risco de informações desatualizadas ou incorretas. A combinação contempla uma solução de código aberto com documentação pública detalhada (Odoo), líderes globais do mercado corporativo (SAP e Oracle/NetSuite) e a documentação do banco de dados que sustenta a parte técnica do ERP (PostgreSQL).

Detalhamento completo: [`fontes/fontes-utilizadas.md`](fontes/fontes-utilizadas.md).

## 7. Diretriz de comportamento da IA

O notebook foi configurado para atuar como **especialista em sistemas ERP, com conhecimentos em desenvolvimento de software e gestão empresarial**, no papel de professor e consultor. Regras principais:

- Utilizar prioritariamente as fontes do notebook e fundamentar as respostas com citações.
- Explicar de forma didática, com exemplos práticos de empresas e processos passo a passo.
- Apresentar exemplos técnicos quando o assunto for desenvolvimento.
- Informar claramente quando as fontes não contiverem a informação e nunca inventar informações ou referências.

Assuntos cobertos: fundamentos e arquitetura de ERP, estoque, vendas/PDV/notas fiscais, compras, financeiro, banco de dados, integração entre módulos e APIs, e relatórios.

Texto completo da diretriz: [`configuracao/diretriz-especialista.md`](configuracao/diretriz-especialista.md).

## 8. Perguntas realizadas e resultados

Roteiro de testes:

| # | Pergunta | Status |
|---|----------|:------:|
| 1 | O que é um ERP e como ele integra os diferentes setores de uma empresa? | ✅ Realizada |
| 2 | Explique passo a passo como funciona uma venda em um ERP, desde o registro no PDV até a atualização do estoque e do financeiro. | ✅ Realizada |
| 3 | Como funciona o controle de estoque em um ERP e quais são os principais cuidados para evitar divergências? | ✅ Realizada |

As respostas obtidas, as fontes citadas e as observações serão registradas em [`perguntas-e-respostas/perguntas-realizadas.md`](perguntas-e-respostas/perguntas-realizadas.md) após a execução dos testes no NotebookLM.

## 9. Materiais gerados

| Material | Formato | Local | Status |
|----------|---------|-------|:------:|
| Mapa mental sobre ERP | PNG | [`materiais/mapa-mental/mapa-mental-erp.png`](materiais/mapa-mental/mapa-mental-erp.png) | ✅ Salvo |
| Apresentação "A Anatomia do Negócio Moderno: como o ERP atua como o sistema nervoso central da sua empresa" | PDF | [`materiais/apresentacao/apresentacao-anatomia-do-negocio-moderno.pdf`](materiais/apresentacao/apresentacao-anatomia-do-negocio-moderno.pdf) | ✅ Salvo |

Mais informações: [`materiais/README.md`](materiais/README.md).

## 10. Evidências do funcionamento

As capturas de tela que comprovam o funcionamento do notebook serão armazenadas em [`evidencias/`](evidencias/):

| Evidência | Pasta | Status |
|-----------|-------|:------:|
| Notebook criado | [`evidencias/notebook/`](evidencias/notebook/) | ⬜ Pendente |
| Fontes adicionadas | [`evidencias/fontes/`](evidencias/fontes/) | ✅ Salva |
| Perguntas, respostas e citações | [`evidencias/respostas/`](evidencias/respostas/) | ⬜ Pendente |

Mais informações: [`evidencias/README.md`](evidencias/README.md).

## 11. Notebook compartilhado

> 🔗 **Link do notebook:** https://notebooklm.google.com/notebook/a10006ca-c732-40d8-aa40-5e177e02e1c3

## 12. Tecnologias e ferramentas

| Tecnologia / Ferramenta | Uso no projeto |
|-------------------------|----------------|
| Google NotebookLM | Criação do segundo cérebro, chat com citações e geração de materiais |
| Gemini | Modelo de IA utilizado pelo NotebookLM |
| Markdown | Documentação do projeto |
| Git | Controle de versão |
| GitHub | Hospedagem e publicação do repositório |

## 13. Estrutura de diretórios

```text
segundo-cerebro-erp/
│
├── README.md                          # Documentação principal do projeto
│
├── fontes/
│   └── fontes-utilizadas.md           # Fontes, justificativas e status de verificação
│
├── configuracao/
│   ├── objetivo.md                    # Objetivo e público-alvo do segundo cérebro
│   └── diretriz-especialista.md       # Instrução de comportamento para o NotebookLM
│
├── perguntas-e-respostas/
│   └── perguntas-realizadas.md        # Roteiro de testes e registro das respostas
│
├── materiais/
│   ├── README.md                      # Descrição dos materiais gerados
│   ├── mapa-mental/                   # Mapa mental exportado (PNG)
│   └── apresentacao/                  # Apresentação de slides (PDF)
│
└── evidencias/
    ├── README.md                      # Descrição e convenções das evidências
    ├── notebook/                      # Prints do notebook criado
    ├── fontes/                        # Prints das fontes adicionadas
    └── respostas/                     # Prints das perguntas, respostas e citações
```

| Pasta | Finalidade |
|-------|------------|
| `fontes/` | Documenta as fontes de referência, a justificativa de cada uma e se foram efetivamente adicionadas ao notebook. |
| `configuracao/` | Guarda o objetivo do projeto e a diretriz (instruções personalizadas) aplicada ao NotebookLM. |
| `perguntas-e-respostas/` | Contém o roteiro de perguntas de teste e o registro das respostas e citações reais. |
| `materiais/` | Armazena os materiais produzidos pelo NotebookLM (mapa mental, apresentação, guias, resumos). |
| `evidencias/` | Armazena capturas de tela que comprovam cada etapa do funcionamento. |

> As pastas vazias contêm um arquivo `.gitkeep` apenas para que o Git as mantenha no repositório. Ele pode ser removido quando os arquivos reais forem adicionados.

## 14. Como reproduzir o projeto

1. **Acesse** o [Google NotebookLM](https://notebooklm.google.com/) com uma conta Google.
2. **Crie um novo notebook** com um nome como "Segundo Cérebro — ERP".
3. **Adicione as fontes** listadas em [`fontes/fontes-utilizadas.md`](fontes/fontes-utilizadas.md):
   - Para sites, utilize a opção de fonte do tipo **Site/URL**.
   - Para vídeos, utilize a opção **YouTube** informando a URL de um vídeo específico do canal.
   - Confira se cada fonte foi processada corretamente e registre o status no arquivo de fontes.
4. **Configure a diretriz**: copie o texto de [`configuracao/diretriz-especialista.md`](configuracao/diretriz-especialista.md) para as instruções personalizadas do chat do notebook.
5. **Execute as perguntas** de [`perguntas-e-respostas/perguntas-realizadas.md`](perguntas-e-respostas/perguntas-realizadas.md), uma por vez.
6. **Verifique as citações** de cada resposta, clicando nelas para confirmar o trecho de origem.
7. **Registre** as respostas, fontes citadas e observações no arquivo de perguntas.
8. **Gere os materiais** (mapa mental e apresentação) pelo painel de estúdio do NotebookLM e salve-os em [`materiais/`](materiais/).
9. **Capture as evidências** de cada etapa e salve-as em [`evidencias/`](evidencias/).
10. **Compartilhe o notebook** (configurando o acesso por link) e insira o link na seção [Notebook compartilhado](#11-notebook-compartilhado).
11. **Publique** as alterações no GitHub.

## 15. Checklist de conclusão

- [x] Criar notebook no NotebookLM.
- [x] Adicionar fontes confiáveis.
- [x] Configurar a diretriz do especialista.
- [x] Realizar as perguntas de teste.
- [ ] Verificar as citações das respostas.
- [x] Gerar mapa mental.
- [x] Gerar apresentação de slides.
- [ ] Salvar evidências.
- [x] Compartilhar o notebook.
- [x] Inserir o link do notebook no README.
- [x] Publicar o repositório no GitHub.

> Marque cada item somente após a existência de evidência correspondente neste repositório.
