# 🎯 PUTSprompts

> Biblioteca modular de prompts estruturados orientados ao framework **PUTS**: Papel, Usuário, Tarefa e Saída.

[![GitHub license](https://img.shields.io/github/license/Ujeverson/PUTSprompts)](./LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](./CONTRIBUTING.md)
[![Prompt Engineering](https://img.shields.io/badge/Framework-PUTS-blue)](https://github.com/Ujeverson/PUTSprompts)

---

## 🧭 Sumário

* [Visão Geral](#-visão-geral)
* [O Método PUTS](#-o-método-puts)
* [Índice de Arquivos e Prompts](#-índice-de-arquivos-e-prompts)
  * [Modelos Base (Templates)](#modelos-base-templates)
  * [Acadêmico & Pesquisa](#acadêmico--pesquisa)
  * [Educação & Ensino](#educação--ensino)
  * [Desenvolvimento de Software](#desenvolvimento-de-software)
  * [Ciência de Dados & Estatística](#ciência-de-dados--estatística)
  * [Produtividade & Gestão](#produtividade--gestão)
  * [Arquivos do Repositório](#arquivos-do-repositório)
* [Como Utilizar](#-como-utilizar)
* [Como Contribuir](#-como-contribuir)
* [Licença](#-licença)

---

## 📌 Visão Geral

O **PUTSprompts** reúne comandos e instruções de alto desempenho desenhados para modelos de linguagem (LLMs). O objetivo do repositório é eliminar ambiguidades na interação com IAs generativas por meio de uma arquitetura consistente, reprodutível e com validação de formato de saída.

---

## 🧠 O Método PUTS

Cada prompt deste repositório segue a estrutura dividida em 4 pilares:

| Pilar | Dimensão | Descrição |
| :--- | :--- | :--- |
| **P** | **Papel** | A identidade, persona ou especialidade que o modelo deve assumir. |
| **U** | **Usuário** | O contexto, público-alvo, premissas e limitações do interlocutor. |
| **T** | **Tarefa** | O objetivo central e a ação executável esperada da IA. |
| **S** | **Saída** | Regras de formato (Markdown, JSON, LaTeX), restrições negativas e tom. |

---

## 📂 Índice de Arquivos e Prompts

Todos os componentes e artefatos disponíveis no repositório:

### Modelos Base (Templates)
* [`templates/template-puts-padrao.md`](./templates/template-puts-padrao.md) — Matriz básica estruturada em blocos PUTS para criação de novos prompts.
* [`templates/template-puts-fewshot.md`](./templates/template-puts-fewshot.md) — Template avançado com blocos de exemplificação guiada (Few-Shot Prompting).
* [`templates/template-puts-chain-of-thought.md`](./templates/template-puts-chain-of-thought.md) — Matriz com raciocínio passo a passo antes da emissão da resposta final.

### Acadêmico & Pesquisa
* [`prompts/academico/fichamento-artigo.md`](./prompts/academico/fichamento-artigo.md) — Extração sintética de teses, metodologias, variáveis e lacunas de artigos científicos.
* [`prompts/academico/revisao-sistematica.md`](./prompts/academico/revisao-sistematica.md) — Triagem de literatura e síntese tabular para meta-análises.
* [`prompts/academico/formatacao-latex.md`](./prompts/academico/formatacao-latex.md) — Conversão e conferência de equações e tabelas complexas em LaTeX puro.

### Educação & Ensino
* [`prompts/educacao/plano-de-aula.md`](./prompts/educacao/plano-de-aula.md) — Criação de planos de aula alinhados à BNCC e competências específicas.
* [`prompts/educacao/rubrica-avaliacao.md`](./prompts/educacao/rubrica-avaliacao.md) — Formulação de matrizes de avaliação com níveis de domínio analíticos.
* [`prompts/educacao/gamificacao-atividades.md`](./prompts/educacao/gamificacao-atividades.md) — Dinâmicas ativas, quizzes e mecânicas de jogos pedagógicos.

### Desenvolvimento de Software
* [`prompts/desenvolvimento/code-review.md`](./prompts/desenvolvimento/code-review.md) — Auditoria de código em busca de code smells, segurança e padrões de projeto.
* [`prompts/desenvolvimento/refatoracao-python.md`](./prompts/desenvolvimento/refatoracao-python.md) — Aplicação de tipagem estática (Type Hints), docstrings PEP 257 e princípios SOLID.
* [`prompts/desenvolvimento/geracao-testes-unitarios.md`](./prompts/desenvolvimento/geracao-testes-unitarios.md) — Cobertura de cenários de borda via `pytest` ou `unittest`.

### Ciência de Dados & Estatística
* [`prompts/ciencia-dados/interpretacao-modelos.md`](./prompts/ciencia-dados/interpretacao-modelos.md) — Análise textual de métricas de classificação (F1, AUC-ROC, matriz de confusão).
* [`prompts/ciencia-dados/otimizacao-sql.md`](./prompts/ciencia-dados/otimizacao-sql.md) — Refatoração de consultas analíticas e desenho de agregações.

### Produtividade & Gestão
* [`prompts/produtividade/ata-executiva.md`](./prompts/produtividade/ata-executiva.md) — Conversão de transcrições de reuniões em planos de ação (5W2H).
* [`prompts/produtividade/briefing-projeto.md`](./prompts/produtividade/briefing-projeto.md) — Estruturação de escopo, riscos e entregáveis técnicos.

### Arquivos do Repositório
* [`README.md`](./README.md) — Documentação central de boas-vindas e governança do repositório.
* [`CONTRIBUTING.md`](./CONTRIBUTING.md) — Diretrizes para submissão e homologação de novos prompts via Pull Request.
* [`LICENSE`](./LICENSE) — Termos de distribuição e uso da base sob licença MIT.

---

## 🚀 Como Utilizar

1. Navegue pelo [Índice de Arquivos](#-índice-de-arquivos-e-prompts) até a categoria correspondente à sua necessidade.
2. Abra o arquivo `.md` desejado e copie o conteúdo bruto da seção **Prompt**.
3. Substitua os campos demarcados entre colchetes (`[Contexto]`, `[Entrada do Usuário]`, etc.) pelas suas variáveis de negócio.
4. Cole o texto completo na interface do seu modelo (Gemini, ChatGPT, Claude) ou integre-o ao fluxo da sua API.

---

## 🤝 Como Contribuir

Contribuições que expandem o repositório são bem-vindas:

1. Faça um Fork do projeto (`git checkout -b feature/novo-prompt-puts`).
2. Utilize obrigatoriamente a base do [`template-puts-padrao.md`](./templates/template-puts-padrao.md).
3. Adicione o link relativo do novo arquivo no sumário do `README.md`.
4. Abra um Pull Request detalhando o caso de uso e exemplos de entrada/saída validados.

---

## 📄 Licença

Este projeto é disponibilizado sob os termos da [Licença MIT](./LICENSE).
