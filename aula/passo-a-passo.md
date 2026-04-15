# Aula: Como Instalar seu Sócio de IA

## O que você vai ter ao final desta aula

Um Claude Code configurado e funcionando como sócio operacional da sua empresa — com memória do seu negócio, seus objetivos, seus clientes e suas prioridades.

---

## PARTE 1 — Instalação

### Passo 1: Instale o VS Code

O VS Code é o programa onde você vai conversar com seu sócio de IA.

1. Acesse: https://code.visualstudio.com
2. Clique em **Download for Windows** (ou Mac)
3. Instale normalmente (next, next, finish)

---

### Passo 2: Instale o Node.js

O Claude Code precisa do Node.js para funcionar.

1. Acesse: https://nodejs.org
2. Baixe a versão **LTS** (a recomendada)
3. Instale normalmente

Para verificar se instalou certo, abra o terminal do VS Code (`Ctrl + '`) e digite:
```
node --version
```
Se aparecer um número (ex: v20.11.0), está funcionando.

---

### Passo 3: Instale o Claude Code

Com o terminal aberto no VS Code, cole este comando e pressione Enter:

```
npm install -g @anthropic-ai/claude-code
```

Aguarde instalar. Quando terminar, verifique:
```
claude --version
```

---

### Passo 4: Crie sua conta Anthropic e configure a API

1. Acesse: https://console.anthropic.com
2. Crie uma conta (pode usar o Google)
3. Vá em **API Keys** → **Create Key**
4. Copie a chave gerada (começa com `sk-ant-...`)
5. No terminal, cole:
```
claude config set apiKey SUA_CHAVE_AQUI
```

> Guarde essa chave em um lugar seguro. Não compartilhe com ninguém.

---

## PARTE 2 — Configurando o repositório da empresa

### Passo 5: Baixe o template

Você vai receber (ou clonar) a pasta `socio-ia-template`. Salve ela em um lugar de fácil acesso no seu computador, por exemplo:

```
Documentos/MinhaEmpresa/
```

---

### Passo 6: Abra a pasta no VS Code

1. Abra o VS Code
2. Clique em **File → Open Folder**
3. Selecione a pasta `socio-ia-template` (ou o nome que você deu)
4. Confirme que confia nos arquivos da pasta quando perguntado

---

### Passo 7: Abra o Claude Code

No terminal do VS Code, digite:
```
claude
```

Pressione Enter. O Claude Code vai iniciar.

---

## PARTE 3 — Primeiro uso: onboarding com seu sócio

### Passo 8: Rode o comando de início

Com o Claude Code aberto, digite exatamente:

```
/start
```

Pressione Enter.

Seu sócio de IA vai se apresentar e começar a fazer perguntas sobre o seu negócio.

---

### Como responder bem

**Seja honesto e detalhado.** Quanto mais você contar, mais o sócio vai entender sua realidade.

Exemplos de respostas boas:

> Pergunta: Qual é o seu maior problema hoje no negócio?
> 
> Resposta ruim: "vender mais"
> 
> Resposta boa: "Tenho dificuldade em converter as pessoas que chegam pelo Instagram. Elas curtem o conteúdo mas não compram. Meu ticket é R$997 e vendo em média 3 por mês."

Quanto mais contexto você der, mais preciso e útil o sócio vai ser.

---

### Passo 9: Confirme o resumo

Ao final do onboarding, o Claude vai apresentar um **resumo do que entendeu** sobre sua empresa.

Leia com atenção. Se algo estiver errado ou faltando, corrija ali mesmo — o sócio vai atualizar a memória.

---

### Passo 10: Veja as primeiras sugestões

O Claude vai sugerir as **3 primeiras ações** para o seu negócio. Analise com calma e decida por qual começar.

---

## PARTE 4 — Uso no dia a dia

### Como conversar com seu sócio

A partir de agora, sempre que abrir o VS Code e digitar `claude` no terminal, seu sócio já vai lembrar de tudo sobre o seu negócio.

Exemplos de pedidos que você pode fazer:

- `"Preciso de 5 ideias de conteúdo para essa semana"`
- `"Me ajuda a escrever um e-mail para minha lista"`
- `"Quero estruturar um processo de onboarding para novos clientes"`
- `"Analisa esse texto e me diz se está bom para converter"`
- `"Me ajuda a montar um script de vendas para o WhatsApp"`

---

### Como o sócio aprende com você

Sempre que você corrigir ele ou der um feedback (`"não era isso"`, `"prefiro assim"`), ele salva na memória para não repetir o erro.

Quanto mais você usa, melhor ele fica.

---

## Dúvidas frequentes

**O sócio vai esquecer o que aprendi?**  
Não. Tudo fica salvo na pasta `memory/` do seu projeto. Enquanto você abrir sempre a mesma pasta, ele vai lembrar.

**Posso usar em mais de um negócio?**  
Sim. Crie uma pasta separada para cada empresa e repita o processo.

**Precisa de internet?**  
Sim. O Claude Code se conecta à API da Anthropic. Você paga pelo uso (geralmente alguns centavos por conversa).

**Quanto custa?**  
O plano Pro do Claude custa $20/mês e inclui uso do Claude Code. Para uso via API, o custo varia pelo volume — para uso normal de empresa pequena, fica em torno de $5–20/mês.

---

## Próximos passos após o onboarding

1. Use o sócio todo dia — quanto mais você usa, mais ele aprende
2. Sempre abra a mesma pasta no VS Code para manter a memória ativa
3. Quando tiver uma decisão importante, pergunte a opinião dele
4. Quando aprender algo novo no negócio, conte para ele — ele vai salvar

---

*Este material faz parte da mentoria de estruturação de empresa com IA.*
