# Instalação rápida

SEFAZ MG: Protesto Inscrito em Dívida Ativa é um servidor MCP remoto hospedado em `https://api.mcp.ai/p_sefaz_mg_protesto`. Você não baixa nem roda nada localmente — só aponta seu cliente pra essa URL.

A auth acontece em runtime: clientes com **OAuth 2.1** (Claude Desktop, Cursor, VS Code recentes) abrem o browser na 1ª chamada (magic-link). Clientes sem OAuth recebem a tool `authenticate` — abra `https://app.mcp.ai/agent-auth`, faça login, copie o JWT e cole no chat.

---

## Claude (Web e Desktop)

[➕ Abrir no Claude e conectar](https://claude.ai/new?modal=add-custom-connector#settings/customize-connectors)

Manual: [claude.ai/customize/connectors](https://claude.ai/customize/connectors?surface=cowork) → **+** → **Adicionar conector personalizado** → `SEFAZ MG: Protesto Inscrito em Dívida Ativa` / `https://api.mcp.ai/p_sefaz_mg_protesto`.

Config file (legado): `~/Library/Application Support/Claude/claude_desktop_config.json` (macOS) ou `%APPDATA%\Claude\claude_desktop_config.json` (Windows):

```json
{ "mcpServers": { "sefaz_mg_protesto": { "type": "http", "url": "https://api.mcp.ai/p_sefaz_mg_protesto" } } }
```

## Cursor

[➕ Instalar no Cursor](cursor://anysphere.cursor-deeplink/mcp/install?name=sefaz_mg_protesto&config=eyJ1cmwiOiJodHRwczovL2FwaS5tY3AuYWkvcF9zZWZhel9tZ19wcm90ZXN0byJ9)

`.cursor/mcp.json`:
```json
{ "mcpServers": { "sefaz_mg_protesto": { "url": "https://api.mcp.ai/p_sefaz_mg_protesto" } } }
```

## VS Code (Copilot Chat)

[➕ Instalar no VS Code](vscode:mcp/install?name=sefaz_mg_protesto&config=%7B%22type%22%3A%22http%22%2C%22url%22%3A%22https%3A%2F%2Fapi.mcp.ai%2Fp_sefaz_mg_protesto%22%7D)

`.vscode/mcp.json`:
```json
{ "servers": { "sefaz_mg_protesto": { "type": "http", "url": "https://api.mcp.ai/p_sefaz_mg_protesto" } } }
```

## Outros clientes MCP

Qualquer cliente com **MCP over HTTP**. URL fixa:

```
https://api.mcp.ai/p_sefaz_mg_protesto
```

Dúvidas? [sefaz_mg_protesto@mcp.ai](mailto:sefaz_mg_protesto@mcp.ai)
