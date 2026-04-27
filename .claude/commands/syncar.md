Salve todo o trabalho desta sessão no GitHub (commit + push).

---

## ETAPA 1 — Diagnóstico do estado atual

Rode em paralelo, sem `cd`:

```bash
git rev-parse --is-inside-work-tree 2>/dev/null
git status --short
git remote -v
git branch --show-current
```

Com base no resultado, decida o caminho:

- **Não é repo git** → vá para "Primeira vez"
- **É repo git mas sem remote** → vá para "Primeira vez (já com git init)"
- **Tem remote configurado** → vá para "Commit + push"

---

## ETAPA 2 — Primeira vez (sem repositório)

1. Pergunte o nome do repositório que ele quer no GitHub e se deve ser **público** ou **privado**.
2. Verifique se o `gh` (GitHub CLI) está disponível:
   ```bash
   gh --version
   ```
3. **Se `gh` estiver instalado e autenticado** (`gh auth status`), crie o repo automaticamente:
   ```bash
   git init
   gh repo create NOME --private --source=. --remote=origin
   ```
   (troque `--private` por `--public` se for o caso)
4. **Se `gh` NÃO estiver disponível**, oriente o caminho manual:
   - Abra `https://github.com/new` e crie o repo
   - Volte ao terminal e rode:
     ```bash
     git init
     git remote add origin https://github.com/USUARIO/REPOSITORIO.git
     ```
5. Siga para "Commit + push".

---

## ETAPA 3 — Commit + push (sempre)

1. Mostre ao fundador um resumo curto do que mudou (use `git status --short`).
2. Pergunte se ele quer incluir tudo ou se tem arquivo sensível pra deixar de fora.
3. Stage:
   ```bash
   git add -A
   ```
   Se ele apontou arquivos sensíveis (`.env`, credenciais, planilhas pessoais), adicione ao `.gitignore` antes do `git add`.
4. Crie o commit com mensagem descritiva sobre **o que foi feito na sessão** (não "update" ou "wip"):
   ```bash
   git commit -m "mensagem clara do que mudou"
   ```
5. Detecte a branch atual e empurre pra ela — **não force `main`**:
   ```bash
   BRANCH=$(git branch --show-current)
   git push -u origin "$BRANCH"
   ```
6. Confirme o sucesso. Se for primeira sincronização, mostre o link do repo:
   ```bash
   gh repo view --web --no-browser 2>/dev/null || git remote get-url origin
   ```

---

## Tratamento de erros

- **Erro de autenticação** → oriente `gh auth login` (se tiver gh) ou criar Personal Access Token em `https://github.com/settings/tokens` e usar como senha no push.
- **Push rejeitado (non-fast-forward)** → puxe primeiro:
  ```bash
  git pull --rebase origin "$BRANCH"
  ```
  Resolva conflitos, e tente o push de novo.
- **Branch remota não existe** → o `-u` no `git push -u origin "$BRANCH"` já cria.

Tom: direto, sem enrolação. Confirma o que foi salvo, mostra o link, fim.
