# 🥷 ShinobiAgent

![ShinobiAgent](assets/ShinobiAgent%2001.png)

## Descrição

**ShinobiAgent** é uma aplicação multiplataforma desktop desenvolvida com Kivy e KivyMD, projetada para rodar discretamente em segundo plano, permitindo a integração direta com o servidor remoto do **AgentNinjas** na Huawei Cloud. Inspirado na tradição dos ninjas operando de forma furtiva e eficiente, o ShinobiAgent sincroniza estados e executa comandos definidos pelo usuário através de sua conta online.

## Principais Funcionalidades

- Execução autônoma de tarefas em segundo plano.
- Sincronização automática e segura com o servidor remoto.
- Monitoramento silencioso e eficiente dos processos locais.
- Armazenamento local de estados para sincronização posterior.
- Comunicação integrada usando protocolo MCP através do módulo **SenseiProtocol**.

## Estrutura do Projeto

```
ShinobiAgent/
├── main.py
├── buildozer.spec
├── SenseiProtocol/
│   ├── sensei_server.py
│   └── tools.py
├── modules/
│   ├── katana_sync.py
│   ├── kage_watcher.py
│   ├── kunai_executor.py
│   ├── shinobi_state.py
│   └── smoke_signal.py
├── assets/
│   ├── icons/
│   └── images/
├── screens/
│   └── LoginScreen.py
└── utils/
    └── helpers.py
```

## Stack Tecnológico

- Python
- Kivy & KivyMD
- LangChain & LangGraph
- MCP (Model Context Protocol)
- Buildozer para compilação multiplataforma

## Como Executar

### Instalação

```bash
python -m venv .venv
source .venv/bin/activate  # Linux/MacOS
.venv\Scripts\activate     # Windows

pip install kivy kivymd langchain langgraph openai langchain-openai langchain-anthropic langchain_community bs4 scikit-learn pandas pyarrow matplotlib lxml mcp[cli]
```

### Execução

```bash
python main.py
```

### Compilação com Buildozer

```bash
buildozer -v android debug
# ou
buildozer -v windows debug
```

## Contribuições

Para sugestões, correções ou novas funcionalidades, crie um pull request seguindo as orientações do projeto.

---

**AgentNinjas © 2025 - Todos os direitos reservados.**
