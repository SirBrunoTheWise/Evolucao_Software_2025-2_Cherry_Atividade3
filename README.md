# Evolução de Software 2025.2 – Cherry Studio
Auditoria de Processos de Integração Contínua (CI) e Entrega Contínua (CD)

## Visão geral
Este repositório contém os artefatos desenvolvidos para a **Atividade 3** da disciplina **Evolução de Software** da Universidade Federal de Sergipe. O objetivo do projeto é realizar uma auditoria técnica detalhada nos processos de automação e Gerência de Mudanças (GM) do projeto open-source **Cherry Studio**.

A análise investiga como a infraestrutura de CI/CD influencia a evolução do software, garantindo a qualidade do código através de *Quality Gates* rigorosos e permitindo uma alta frequência de releases em um ambiente desktop complexo.

## Projeto analisado
O projeto analisado é o **Cherry Studio**, um agente de Inteligência Artificial para desktop construído com a plataforma Electron. A escolha deve-se à sua arquitetura moderna e ao uso extensivo de GitHub Actions para orquestrar builds multiplataforma.

- **Repositório oficial:** [https://github.com/CherryHQ/cherry-studio](https://github.com/CherryHQ/cherry-studio)
- **Stack principal:** Electron, Node.js (pnpm), TypeScript, React.

## Objetivos do trabalho
- Mapear a infraestrutura de automação e os workflows do projeto.
- Classificar o nível de maturidade de CI/CD (Cenário A).
- Avaliar a eficiência do pipeline com base em métricas de tempo de feedback e confiabilidade.
- Discutir o impacto da automação na gestão da dívida técnica e na facilidade de contribuição para novos desenvolvedores.

## Ferramentas e Tecnologias Identificadas
A auditoria identificou um ecossistema robusto focado em performance e segurança:

### Orquestração e Qualidade Estática
- **GitHub Actions:** Orquestração de 16 workflows (CI, CD, Nightly Builds).
- **pnpm:** Gerenciamento de dependências focado em velocidade e economia de disco.
- **Oxlint & ESLint:** Ferramentas de linting para garantir padrões de codificação.
- **TypeScript:** Verificação de tipos para prevenir erros em tempo de execução.

### Suíte de Testes e Build
- **Vitest:** Framework de testes unitários e de integração de alta performance.
- **Playwright:** Automação de testes de ponta a ponta (E2E) para a interface Electron.
- **Electron Builder:** Automação do empacotamento e assinatura de executáveis (.exe, .dmg, .deb).

### Automação de Vanguarda
- **Claude Code Review:** Workflow de revisão de código assistida por IA.
- **Auto-i18n:** Pipeline automatizado para internacionalização e traduções.

## Estrutura do repositório
```bash
Evolucao_Software_2025-2_Cherry_Atividade1
│
├─ documentos
│  └─ Relatorio_Auditoria_CICD_Cherry.pdf # Documento completo da auditoria
│
├─ figuras
│  ├─ fluxograma_pipeline.png             # Desenho do fluxo de CI
│  ├─ evidencias_github.png               # Prints da pasta .workflow
│  
│
└─ README.md
