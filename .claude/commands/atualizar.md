---
description: Sincroniza memory/, _contexto/, marca/ e catalogo de ferramentas — mantém o sócio afiado
---

Varra o projeto inteiro e atualize todos os arquivos de contexto que ficaram desatualizados.

## ETAPA 1 — Mapear o estado atual

Leia em ordem:

1. `memory/MEMORY.md` e todos os `.md` em `memory/`
2. `_contexto/` (todos os arquivos)
3. `marca/` (todos os arquivos)
4. `templates/ferramentas/catalogo.md`
5. Liste o que existe em `operacoes/`, `conteudo/`, `dados/` (apenas estrutura, não precisa abrir tudo)

## ETAPA 2 — Detectar inconsistências

Compare o que está nos arquivos de memória com:

- Pastas e projetos novos que apareceram em `operacoes/projetos/`
- Conteúdo recente em `conteudo/` (carrosseis, roteiros) que sugira mudança de canal/posicionamento
- Relatórios em `dados/relatorios/` que mostrem números diferentes dos registrados em `memory/numeros.md`

Liste o que está:

- **Desatualizado** (existe mas a info mudou)
- **Faltando** (precisa existir e não existe)
- **Conflitante** (dois arquivos dizem coisas diferentes sobre o mesmo tema)

## ETAPA 3 — Atualizar

Pergunte ao fundador o que mudou desde a última atualização (faturamento, novas operações, ferramentas adicionadas, mudança de meta) e atualize:

- `memory/MEMORY.md` — índice (adicione entradas faltando)
- Arquivos individuais em `memory/` — informações que mudaram
- `_contexto/` — referências desatualizadas
- `marca/` — guia de marca, se houver mudança
- **`templates/ferramentas/catalogo.md`** — adicione/remova CLIs, MCPs, APIs, ferramentas SaaS de negócio. Cheque se ferramentas instaladas refletem a realidade rodando:
  ```bash
  claude --version 2>/dev/null
  vercel --version 2>/dev/null
  gh --version 2>/dev/null
  git --version
  ```

## ETAPA 4 — Relatório

Apresente:

- ✅ **O que foi atualizado**
- ➕ **O que foi criado**
- ⚠️ **O que ficou pendente** (perguntas em aberto pro fundador)
- 🟰 **O que ficou igual**

Se encontrar inconsistências importantes (metas batidas e não atualizadas, operação que sumiu, ferramenta nova não registrada), destaque e pergunte como ele quer resolver — não decida sozinho em informação crítica.

Tom: direto, de sócio fazendo limpeza de mesa antes de planejar a próxima rodada.
