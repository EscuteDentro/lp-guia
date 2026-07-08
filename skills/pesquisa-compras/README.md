# Skill: /pesquisa-compras

Assistente de compras multi-plataforma para o Claude Code.

**Status:** funcional — precisa de melhorias (ver notas abaixo).

## O que faz

Pesquisa preços em Mercado Livre, Shopee, Amazon, Magazine Luiza, Estante Virtual (livros) e encartes de supermercado. Inclui pré-pesquisa de reviews e alternativas, frete estimado para um CEP configurável, parcelamento sem juros, cupons e flag de envio internacional com estimativa de imposto.

## Configurar antes de usar

Editar `SKILL.md` e substituir `{SEU_CEP}` pelo seu CEP e `{SUA_CIDADE}` pela sua cidade.

## Como instalar

Copiar esta pasta para `.claude/skills/pesquisa-compras/` no seu projeto e adicionar um command em `.claude/commands/pesquisa-compras.md` apontando para o SKILL.md.

## Notas e melhorias pendentes

- Dependência de scripts Python externos (`buscar.py`, `gerar-html.py`) — precisam ser copiados manualmente para o projeto
- CLIs de algumas plataformas requerem autenticação prévia (Mercado Livre OAuth)
- Algumas plataformas têm scraping instável; resultados podem variar
- Sem testes automatizados
