# Convite de Casamento — Pedro Henrique & Joyce Kelly

Convite digital em página única. Basta abrir o `index.html` no navegador
ou publicar a pasta (GitHub Pages, Netlify, etc.).

**28 de novembro de 2026 · Pontal/SP**

## Estrutura

```
index.html        → o convite inteiro (HTML + CSS + JS, sem dependências)
assets/           → fotos e monograma (veja assets/LEIA-ME.md)
```

## O que tem no convite

Capa animada de álbum · Hero com monograma · Música (YouTube) · Versículo ·
Nosso convite · Linha do tempo do dia · Informações · Como chegar (com mapas) ·
Dress code e cores reservadas · Contagem regressiva · Lista de presentes + Pix ·
Confirmação de presença por WhatsApp

## Como editar as informações

Tudo o que muda com frequência está reunido no bloco **★ EDITE AQUI ★**,
no início do `<script>` no fim do `index.html`:

| Variável | Para que serve |
|---|---|
| `DATA_ISO` | data/hora usada na contagem regressiva |
| `DATA_EXTENSO`, `DATA_CURTA` | como a data aparece escrita |
| `NOIVOS` | nomes usados nas mensagens de WhatsApp |
| `WHATSAPP_NUM` | número que recebe as confirmações (só números, com 55 + DDD) |
| `WHATSAPP_EXIBE` | esse mesmo número, como aparece escrito no convite |
| `PIX_TIPO`, `PIX_KEY`, `PIX_COPIA`, `PIX_NOME` | dados do Pix |
| `LINK_PRESENTES` | link da lista de presentes |
| `MUSICA_YT_ID`, `MUSICA_TITULO` | música do convite (ID do vídeo no YouTube) |

### Confirmação de presença

Um botão só: **Confirmar pelo WhatsApp**. Ele abre a conversa com
`WHATSAPP_NUM` com a mensagem já escrita — o convidado só toca em enviar.
O número também aparece clicável logo abaixo.

Não há formulário: quem confirma se identifica pelo próprio WhatsApp, e o
convite não promete que a presença está confirmada, porque a página não tem
como saber se a mensagem foi enviada.

Para mudar o texto da mensagem, edite a função `linkWhatsApp()`.

### Fotos

Monograma, foto do casal e foto da recepção já estão no ar. Falta apenas a
**foto da cerimônia** (`assets/cerimonia.jpg`) — é só colocar o arquivo na pasta
`assets/` com esse nome que ela aparece sozinha.

Detalhes em `assets/LEIA-ME.md`.

## Paleta — Verde Menta

| Token | Cor | Uso |
|---|---|---|
| `--cream` | `#f3f8f5` | fundo |
| `--pistache-soft` | `#d6ecdf` | menta pálido |
| `--pistache` | `#a8d5c0` | bordas e filetes |
| `--musgo` | `#7cb49a` | verde menta (destaque) |
| `--musgo-dark` | `#3d7a61` | verde profundo (títulos, botões) |

As cores ficam em `:root`, no topo do `<style>` — mudar ali muda o convite todo.
