# Auditoria de Maturidade em Ecossistemas LLM

---

## Sumário

- Sobre o Repositório
- Projeto Analisado
- Equipe
- Estrutura da Auditoria
- Metodologia
- Vídeo de Apresentação

---

## Sobre o Repositório

Este repositório resistra todos os passos e conclusões feitas pela equipe na Atividade Avaliativa 1 (A1), onde o objetivo é realizar uma auditoria técnica de maturidade de processo em um projeto open source baseado em LLMs, usando como referência os modelos CMMI-DEV v2.0 e MPS.BR (MR-MPS-SW).

---

## Projeto Analisado

O projeto analisado foi o **Crawl4AI** — https://github.com/unclecode/crawl4ai

O Crawl4AI é uma biblioteca open source em Python que realiza web crawling e scraping com saída otimizada para modelos de linguagem. Em vez de retornar HTML bruto, o projeto converte o conteúdo das páginas em Markdown limpo e estruturado, removendo scripts, anúncios e tags desnecessárias, facilitando o consumo do conteúdo por LLMs em pipelines de RAG, agentes de IA e sistemas de extração de dados.

---

- Linguagem principal - Python
- Licença - Apache 2.0
- Última versão - v0.8.5 (18 de março)

---

## Equipe

**Equipe**

---

- Pedro Afonso Tavares Barreto da Silva - 202300027580
- Jose Valter de Oliveira Junior - 202300083678
- Yasmin Silva Santos - 202300084058
- Beatriz Eduarda Pires da Cruz - 202200092647
- João Guilherme Santos Florêncio - 202200025546

---

## Estrutura da Auditoria

A auditoria está dividida em cinco tópicos. Os arquivos estão organizados da seguinte forma:

ES_2026-1_Crawl4AI/
├── README.md
├── Ciclo de Vida e Metodologias Ágeis.md
├── Engenharia de Requisitos.md
├── Arquitetura e Modelagem.md
├── Verificação e Validação.md
├── Qualidade de Software.md
└── imagens/

---

## Metodologia

A análise foi conduzida diretamente no repositório do Crawl4AI no GitHub, com inspeção de issues, pull requests, releases, workflows de CI/CD e arquivos de documentação. Cada tópico foi avaliado segundo os critérios do CMMI-DEV v2.0 e do MPS.BR.

Tópico - Área de Processo - Alinhamento
I. Ciclo de Vida e Metodologias Ágeis - Gerência de Projetos (GPR) - CMMI: Planejamento, Monitoramento e Controle / MPS.BR
II. Engenharia de Requisitos - Gerência de Requisitos (GRE) - CMMI: REQM / MPS.BR
III. Arquitetura e Modelagem - Projeto e Construção (PJR) - CMMI: Solução Técnica / MPS.BR
IV. Verificação e Validação - V&V | CMMI: VER/VAL / MPS.BR
V. Qualidade de Software - Garantia da Qualidade (GQA) - CMMI: PPQA / MPS.BR

---

## Vídeo de Apresentação