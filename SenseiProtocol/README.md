# 🥷 SenseiProtocol

![SenseiProtocol](../assets/SenseiProtocol%2001.png)

## Descrição

**SenseiProtocol** é o módulo interno do ShinobiAgent que implementa o Model Context Protocol (MCP). Inspirado pela sabedoria profunda dos mestres ninjas, este módulo atua como um provedor inteligente e tecnológico, oferecendo ferramentas e contextos avançados para os modelos de linguagem (LLMs), garantindo que as respostas e decisões dos agentes sejam bem fundamentadas e precisas.

SenseiProtocol facilita a integração transparente com ferramentas externas e fornece uma interface padronizada para comunicação entre agentes e recursos digitais.

## Principais Funcionalidades

- Integração completa com MCP (Model Context Protocol).
- Fornecimento de contexto e ferramentas avançadas para LLMs.
- Comunicação eficiente com agentes externos (Claude Desktop, Cursor, Windsurf).
- Recuperação eficiente e precisa de documentação técnica e informações via LangGraph.

## Estrutura do Projeto

```
SenseiProtocol/
├── sensei_server.py
├── tools.py
└── resources/
    └── docs/
```

## Tecnologias

- Python
- MCP (Model Context Protocol)
- LangChain & LangGraph
- OpenAI Embeddings

## Como Executar

### Instalação de Dependências

```bash
pip install langchain langgraph langchain-openai langchain-anthropic langchain_community openai scikit-learn bs4 pandas pyarrow matplotlib lxml mcp[cli]
```

### Execução do Servidor MCP

```bash
python sensei_server.py
```

## Integração com Ferramentas Externas

Configure suas ferramentas (Claude Desktop, Cursor, Windsurf) conforme documentação MCP oficial, usando o servidor configurado em:

```json
{
  "mcpServers": {
    "senseiprotocol": {
      "command": "python",
      "args": ["sensei_server.py"],
      "env": {"OPENAI_API_KEY": "sua-chave-openai"}
    }
  }
}
```

## Contribuições

Envie sugestões, melhorias ou novas funcionalidades através de pull requests seguindo as orientações do projeto.

---

**SenseiProtocol © 2025 - Todos os direitos reservados.**