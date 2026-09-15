# Fotos do convite

## Situação atual

| Arquivo                 | Onde aparece                              | Status |
|-------------------------|-------------------------------------------|--------|
| `monograma.png`         | Capa (álbum) e topo do convite            | ✅ no ar |
| `casal.jpg`             | Hero — logo abaixo de "Convidam você"     | ✅ no ar |
| `recepcao.jpg`          | Card da **recepção**, abaixo do endereço  | ✅ no ar |
| `igreja.jpg`            | Card da **cerimônia**, abaixo do endereço | ⬜ falta enviar |
| `casal-original.jpg`    | (só arquivo — a foto do casal sem corte)  | guardado |

## Como enviar a foto que falta

Coloque o arquivo **nesta pasta** (`assets/`), com **exatamente** o nome
`igreja.jpg` (minúsculo, sem acento). O convite já procura por ele — assim
que o arquivo existir, a foto aparece sozinha, sem mexer em código.

Sugestão: foto **horizontal** (paisagem), por volta de 1000 × 700px.
Ela é exibida em proporção 4:3, cortada pelo centro.

## Enquanto uma foto não é enviada

Nada quebra. O convite se ajusta sozinho:

- **Monograma ausente** → aparece um monograma "P & J" em verde menta.
- **Foto ausente** → o espaço dela simplesmente não é exibido.

## Reenquadrar a foto do casal

`casal.jpg` é um recorte 3:4 de `casal-original.jpg`, feito para o casal
preencher a moldura em arco do hero. Para mudar o enquadramento, recorte de
novo a partir de `casal-original.jpg` mantendo a proporção 3:4 e salve como
`casal.jpg`.

Para um ajuste fino sem recortar, dá para mexer no `object-position` da regra
`.hero-photo-frame img`, no `index.html` (ex.: `center 40%` sobe o corte).

## Dicas de arquivo

- **`monograma.png`**: PNG com **fundo transparente** — é o que faz ele se
  integrar ao fundo da capa sem uma caixa branca em volta.
- Mantenha cada arquivo abaixo de ~300 KB para o convite abrir rápido no 4G.
