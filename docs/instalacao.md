# Instalação detalhada

SEFAZ MG: Protesto Inscrito em Dívida Ativa é um servidor MCP remoto. Aponte seu cliente pra `https://api.mcp.ai/p_sefaz_mg_protesto`. Snippets rápidos: [INSTALL.md](../INSTALL.md).

| Cliente | URL | Auth |
|---|---|---|
| Claude Desktop | `https://api.mcp.ai/p_sefaz_mg_protesto` | OAuth 2.1 ou agent-auth |
| Cursor | `https://api.mcp.ai/p_sefaz_mg_protesto` | OAuth 2.1 ou agent-auth |
| VS Code (Copilot) | `https://api.mcp.ai/p_sefaz_mg_protesto` | OAuth 2.1 ou agent-auth |

A config JSON é a mesma em todos: só a URL, sem headers.

## Desinstalar

Remova o bloco `mcpServers.sefaz_mg_protesto` (ou `servers.sefaz_mg_protesto` no VS Code) do config do cliente e reinicie.
