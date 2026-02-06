# Relatório de Capacidades do Sistema Antigravity

Este documento detalha todas as ferramentas, servidores MCP conectados e habilidades especializadas (Skills) disponíveis no ambiente atual.

## 1. Servidores MCP Conectados
O Model Context Protocol (MCP) conecta o sistema a ferramentas e dados externos. Os seguintes servidores estão ativos:

| Servidor MCP | Descrição |
| :--- | :--- |
| **context7** | Motor de busca de documentação técnica e exemplos de código para qualquer biblioteca/framework. |
| **github-mcp-server** | Integração com GitHub para gestão de repositórios, issues, PRs e workflows. |
| **gmp-code-assist** | Assistente da Google Maps Platform para documentação e implementação de mapas. |
| **notebooklm** | Integração com Google NotebookLM. **Motor do "Antigravity Brain":** 12 Bases de Conhecimento curadas para pesquisa técnica grounded. |
| **notion-mcp-server** | Conexão com Notion para gestão de páginas, bancos de dados e comentários. |
| **supabase-mcp-server** | Ferramentas para gestão de projetos Supabase, banco de dados e edge functions. |
| **TestSprite** | Agente especialista em testes de software e validação automática. |


---

## 2. The Antigravity Brain (Conhecimento Grounded)
O sistema possui uma camada de "Grounding" composta por **12 Cadernos de Conhecimento** hospedados no NotebookLM, contendo +220 fontes oficiais (docs, whitepapers, engineering blogs). O `skill-evolution-engine` consulta estas bases antes de recorrer à web aberta.

**Categorias Monitoradas:**
1.  **IA & Agentes** (LangChain, CrewAI, RAG)
2.  **Web Fullstack** (React, Next.js, Node)
3.  **Mobile & Bots** (Flutter, Telegram, Whatsapp)
4.  **Linguagens & Core** (Python, TS, Rust, Go)
5.  **Cloud & DevOps** (AWS, Docker, K8s)
6.  **Segurança** (Pentest, AppSec, NetSec)
7.  **Dados & Analytics** (Data Eng, Vector DBs)
8.  **Marketing & Growth** (SEO, Copy, Analytics)
9.  **Product & Design** (UX/UI, Figma, Product Mgmt)
10. **Engenharia de Software** (Architecture, Patterns)
11. **Automação & Workflows** (n8n, Playwright)
12. **Blockchain & Web3** (Solidity, Ethereum)
Ferramentas intrínsecas do agente para interação com o sistema operacional e ambiente de desenvolvimento.

### Manipulação de Arquivos e Código
*   `write_to_file`: Criar novos arquivos.
*   `view_file`: Ler conteúdo de arquivos.
*   `replace_file_content`: Editar blocos contíguos de código.
*   `multi_replace_file_content`: Múltiplas edições em um arquivo.
*   `view_file_outline`: Ver estrutura de classes e funções de um arquivo.
*   `view_code_item`: Ver definições específicas de código.
*   `find_by_name`: Buscar arquivos por nome/padrão.
*   `grep_search`: Busca textua/regex dentro de arquivos.
*   `list_dir`: Listar diretórios.

### Execução e Terminal
*   `run_command`: Executar comandos de terminal (PowerShell/Bash).
*   `send_command_input`: Interagir com comandos em execução.
*   `read_terminal`: Ler saída de terminais.
*   `command_status`: Verificar status de comandos em background.

### Navegação e Pesquisa
*   `search_web`: Pesquisar na internet (Google Search).
*   `read_url_content`: Ler conteúdo de texto de URLs.
*   `browser_subagent`: Navegador autônomo para interações complexas na web.

### Geração de Mídia
*   `generate_image`: Criar imagens e assets visuais.

---

## 3. Habilidades Especializadas (Skills)
Skills são pacotes de conhecimento especializado para tarefas complexas.
### ⚙️ System & Meta-Skills (Core)
*   **Skill Evolution Engine:** `skill-evolution-engine` (Custodian). Atualiza e audita o ecossistema automaticamente, priorizando a Base de Conhecimento.
*   **Skill Factory:** `skill-factory-universal` (Architect). Cria novas skills seguindo padrões v5.0 (segurança, tipagem, modularidade).
*   **Utilitários:** `universal-translator`, `using-superpowers`.

### 🧠 IA, Agentes e LLMs
*   **Agentes Autônomos:** `agent-orchestrator`, `agent-evaluation`, `agent-memory-systems`, `crewai`, `langchain-architecture`, `langgraph`, `computer-use-agents`, `subagent-architect`.
*   **Engenharia de Prompt:** `prompt-architect`, `prompt-library`, `prompt-caching`, `llm-application-dev-prompt-optimize`.
*   **RAG & Vetores:** `rag-engineer`, `vector-database-engineer`, `embedding-strategies`, `hybrid-search-implementation`.
*   **Voz & Áudio:** `voice-agents`, `voice-ai-development`, `fal-audio`.

### 🛡️ Cibersegurança e Hacking Ético
*   **Testes de Invasão (Pentest):** `pentest-checklist`, `pentest-commands`, `ethical-hacking-methodology`, `burp-suite-testing`, `metasploit-framework`, `red-team-tactics`, `kali-linux-tools`.
*   **Web & API Security:** `api-fuzzing-bug-bounty`, `sql-injection-testing`, `xss-html-injection`, `broken-authentication`, `idor-testing`, `top-web-vulnerabilities`.
*   **Infraestrutura & Cloud:** `aws-penetration-testing`, `cloud-penetration-testing`, `active-directory-attacks`, `linux-privilege-escalation`, `windows-privilege-escalation`.
*   **Análise & Engenharia Reversa:** `reverse-engineer`, `malware-analyst`, `binary-analysis-patterns`, `wireshark-analysis`, `memory-forensics`.
*   **Auditoria:** `security-auditor`, `threat-modeling-expert`, `smart-contract-audit`.

### 💻 Desenvolvimento de Software
*   **Frontend:** `frontend-developer`, `react-patterns`, `nextjs-best-practices`, `tailwind-patterns`, `vue-pro`, `angular-migration`, `accessibility-compliance`.
*   **Backend:** `backend-architect`, `nodejs-backend-patterns`, `python-pro`, `java-pro`, `golang-pro`, `rust-pro`, `csharp-pro`, `api-design-principles`, `graphql-architect`.
*   **Mobile:** `mobile-developer`, `flutter-expert`, `react-native-architecture`, `ios-developer`.
*   **Game Dev:** `game-development`, `unity-developer`, `godot-gdscript-patterns`, `unreal-engine-cpp-pro`.
*   **Banco de Dados:** `db-architect-master`, `postgres-best-practices`, `nosql-expert`, `neo4j-cypher`, `sql-optimization-patterns`.

### ☁️ DevOps, Cloud e Infraestrutura
*   **Cloud Providers:** `aws-serverless`, `gcp-cloud-run`, `azure-functions`, `multi-cloud-architecture`.
*   **Container & Orquestração:** `docker-expert`, `kubernetes-architect`, `helm-chart-scaffolding`.
*   **IaC & Automação:** `terraform-specialist`, `ansible-automation`, `github-actions-templates`, `gitlab-ci-patterns`.
*   **Observabilidade:** `observability-engineer`, `prometheus-configuration`, `grafana-dashboards`, `distributed-tracing`.

### 🚀 Negócios, Marketing e Startups
*   **Startups:** `startup-analyst`, `startup-financial-modeling`, `pitch-deck-creator`, `market-sizing-analysis`.
*   **Marketing & SEO:** `seo-audit`, `seo-content-writer`, `content-marketer`, `social-content`, `paid-ads`, `copywriting`.
*   **Produto:** `product-manager-toolkit`, `pricing-strategy`, `launch-strategy`, `user-interview-analysis`.

### 📄 Documentação e Produtividade
*   **Documentação:** `docs-architect`, `api-documenter`, `c4-architecture`, `mermaid-expert`.
*   **Formatos de Arquivo:** `pdf`, `xlsx`, `docx`, `pptx`.
*   **Ferramentas Pessoais:** `obsidian-clipper`, `notion-template-business`.

---

Este documento serve como referência central para todas as capacidades ativas no sistema Antigravity.