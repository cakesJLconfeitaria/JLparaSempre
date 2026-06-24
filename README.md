# Jonas & Larissa 💌

Página do casal — pronta pra hospedar no GitHub Pages.

## Estrutura

```
seu-repositorio/
├── index.html        ← a página
└── imagens/
    ├── foto1.jpg
    ├── foto2.jpg
    ├── foto3.jpg
    └── ...           ← quantas você quiser
```

## Como hospedar no GitHub Pages

1. Crie um repositório no GitHub (pode ser público, ou então `seuusuario.github.io` se quiser usar o domínio raiz).
2. Faça upload do `index.html` e da pasta `imagens/` com as fotos.
3. Vá em **Settings → Pages**.
4. Em **Source**, escolha `Deploy from a branch` → `main` → `/ (root)` → **Save**.
5. Em alguns segundos sua página estará no ar em `https://seuusuario.github.io/nome-do-repo/`.

## Adicionando fotos

Coloque as fotos dentro da pasta `imagens/` numeradas em sequência a partir de 1:

- `foto1.jpg`, `foto2.jpg`, `foto3.jpg`, …

Formatos aceitos: **.jpg, .jpeg, .png, .webp** (a página detecta automaticamente).

A página vai carregando as fotos até encontrar um número que não exista — então as fotos precisam estar numeradas **sem pular números** (foto1, foto2, foto3… e não foto1, foto3, foto5).

**Dica:** comprima as fotos antes de subir (use [squoosh.app](https://squoosh.app/) ou similar). 50 fotos de 200KB cada = 10MB total, carrega tranquilo. 50 fotos de 5MB cada = 250MB, vai ficar lento.

## Trocando a música

Abra o `index.html` e procure por `0tgVpDi06FyKpA1z0VMD4v`. Esse é o ID da música no Spotify (atualmente "Perfect" do Ed Sheeran).

Pra trocar:
1. Abra a música no Spotify (app ou web).
2. Clique nos três pontinhos → **Compartilhar → Copiar link da música**.
3. O link vai ser tipo `https://open.spotify.com/track/SEU_ID_AQUI?si=...`
4. Copie só o `SEU_ID_AQUI` e substitua o ID que está no `index.html`.

## Trocando as datas

No `index.html`, procure pela linha:

```js
var events = {
  kiss:   new Date(2012, 9,  15, 21, 0, 0),
  namoro: new Date(2013, 4,  1,  20, 0, 0)
};
```

Formato: `new Date(ano, mês, dia, hora, minuto, segundo)`.
**Atenção:** mês é zero-indexado — janeiro = 0, fevereiro = 1, …, dezembro = 11.

Também troque os textos abaixo dos cronômetros (procure por "15 de outubro" e "1 de maio").

## Trocando o tema padrão

A página abre no tema **Clássica** por padrão. O usuário pode trocar pelo botão no canto superior direito, e a escolha fica salva no navegador.

Pra mudar o padrão pra Polaroid, troque `class="theme-classic"` por `class="theme-polaroid"` na tag `<body>`.
