# Claude Code OS 🐀
### O sistema operacional da sua empresa — feito pra rodar com IA

Feito pelo Ratos de IA pra alunos do curso Claude Code OS.

> Pensa assim: você acabou de desbloquear um personagem novo no seu negócio.  
> Ele não cansa, não esquece, não pede aumento — e trabalha enquanto você dorme.  
> Esse é o seu novo sócio de IA. Agora é só instalar.

---

## ⚙️ Instalação — escolhe o seu modo

### Modo Fácil — deixa o Claude fazer tudo

Com o Claude Code aberto em qualquer pasta, cola esse prompt e aperta Enter:

```
Instala pra mim o repositório https://github.com/Geeknosnegocios/geek-os-claude.git na pasta atual, abre ela e roda /setup
```

Ele clona, entra na pasta e já inicia a configuração. Você não precisa digitar mais nada.

---

### Modo Terminal — pra quem quer ver a mágica acontecer

**1. Clone o repositório**

```bash
git clone https://github.com/Geeknosnegocios/geek-os-claude.git
cd geek-os-claude
```

**2. Abre no VS Code**

```bash
code .
```

**3. Abre o terminal integrado**

`Ctrl + \`` no Windows · `Cmd + \`` no Mac

```bash
claude
```

**4. Inicializa o sistema**

```
/setup
```

O Claude vai te entrevistar sobre o seu negócio e montar tudo do zero.  
Em 5 minutos você tem um sócio configurado com a realidade da sua empresa.

---

## 🎮 Skills — seus poderes desbloqueados

Pensa nas skills como habilidades especiais do seu personagem.  
Cada uma resolve uma tarefa específica. Você chama, ele executa.

| Skill | O que faz |
|---|---|
| `/setup` | **Comece aqui** — entrevista sobre o negócio e configura tudo |
| `/iniciar` | Liga o sócio no começo do dia com contexto carregado |
| `/syncar` | Salva tudo no GitHub — commit + push automático |
| `/carrossel` | Gera carrossel completo pra Instagram e TikTok |
| `/proposta-comercial` | Proposta profissional em HTML a partir de um briefing |
| `/publicar-site` | Sobe qualquer HTML no ar com link compartilhável |
| `/slide` | Card visual pra apresentação ou post |
| `/analisar-dados` | Lê planilha ou arquivo e gera relatório executivo |
| `/roteiro-post` | Transforma ideia em roteiro de post, reels ou vídeo |
| `/email-profissional` | Email com assunto + CTA pronto pra enviar |
| `/atualizar` | Sincroniza toda a memória do projeto |
| `/novo-projeto` | Abre novo projeto com CLAUDE.md dedicado |

---

## 🗂️ A estrutura que o `/setup` monta pra você

```
_contexto/                          → a cabeça do seu negócio — tudo que o sócio precisa saber
marca/                              → identidade visual, tom de voz, posicionamento
templates/ferramentas/catalogo.md   → arsenal disponível: APIs, CLIs e MCPs
dados/                              → drop zone — joga aqui CSV, XLSX, PDF pra analisar
```

> Não tem MCP do Google Drive? Sem drama.  
> Exporta o arquivo, joga na pasta `dados/` e roda `/analisar-dados dados/seu-arquivo.csv`

---

## 🧠 Como o sócio aprende

Cada vez que você corrige ele, ele salva.  
Cada vez que você conta algo novo sobre o negócio, ele guarda.  
A memória fica na pasta `memory/` — enquanto você abrir a mesma pasta, ele lembra de tudo.

Quanto mais você usa, mais afiado ele fica. É como subir de nível.

---

## 🆘 Travou?

Assiste a **Aula 1.3** do curso — ela cobre a instalação do zero.

Ainda com dúvida: [ratosdeia.com.br](https://ratosdeia.com.br)
