Salve todo o trabalho desta sessão no GitHub (commit + push).

### Se for a primeira vez (sem repositório remoto configurado):

1. Pergunte o nome do repositório que ele quer criar no GitHub
2. Verifique se o git está inicializado na pasta — se não estiver, rode `git init`
3. Instrua a criar o repositório no GitHub (github.com/new) e cole o remote:
   ```
   git remote add origin https://github.com/USUARIO/REPOSITORIO.git
   ```
4. Prossiga para o commit e push

### Sempre:

1. Rode `git status` para ver o que mudou
2. Mostre ao fundador um resumo do que será salvo
3. Faça `git add .`
4. Crie um commit com mensagem descritiva sobre o que foi feito na sessão
5. Rode `git push origin main` (ou a branch correta)
6. Confirme que deu certo e informe o link do repositório

Se der erro de autenticação, oriente a usar um Personal Access Token do GitHub.
