Publique um arquivo HTML no ar e gere um link compartilhável — mas antes, questione o contexto estratégico.

### Antes de executar — pergunte como sócio:

1. Qual é o arquivo HTML que quer publicar? (caminho ou nome)
2. Tem algum nome preferido para a URL?
3. **Para que serve esse site?** (captura de leads, oferta, evento, teste de copy, página de vendas?)
4. **Já tem tráfego planejado para ele?** Se não, publicar sem tráfego é esforço sem retorno — aponte isso diretamente.

Se a resposta da pergunta 3 mostrar uma oportunidade de receita clara, vá em frente e execute com velocidade. Se mostrar algo difuso ou sem fundo de funil definido, diga antes de publicar.

### Execute a publicação usando Vercel CLI:

Verifique se o Vercel CLI está instalado:
```bash
vercel --version
```

Se não estiver, instale:
```bash
npm install -g vercel
```

Faça o deploy:
```bash
vercel [caminho-do-arquivo-ou-pasta] --yes
```

### Entregue:

- O link público gerado (ex: `https://nome.vercel.app`)
- Confirmação de que o site está no ar
- Instrução de como atualizar se precisar republicar
- **Se houver oportunidade óbvia de melhorar a conversão** (CTA fraco, sem captura, sem pixel), aponte — não deixe passar

Se der erro de autenticação no Vercel, oriente a rodar `vercel login` primeiro.
