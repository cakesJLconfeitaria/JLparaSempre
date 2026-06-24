# Jonas & Larissa 💌

Página do casal — pronta pra hospedar no GitHub Pages. **4 temas** com seletor no canto superior direito.

## Os temas

| Tema | Vibe |
|------|------|
| **Clássica** | Creme, bordô e dourado, tipografia serifada em itálico |
| **Polaroid** | Papel retrô, fotos como polaroids rotacionadas, letra manuscrita |
| **Estrelado** | Céu noturno com estrelas piscando e estrelas cadentes, dourado e lavanda ✨ |
| **Jardim** | Verde sálvia e rosa, leve e orgânico |

O tema escolhido fica salvo no navegador de quem visita.

## Estrutura dos arquivos

```
seu-repositorio/
├── index.html        ← a página
├── foto1.jpg
├── foto2.jpg
├── foto3.jpg
└── ...               ← quantas fotos quiser (na raiz, modo teste atual)
```

> Atualmente o código procura as fotos na **raiz** (modo teste). Quando quiser organizar numa pasta `imagens/`, me avisa que eu troco — ou troque você: no `index.html` procure `'foto'+i` e mude pra `'imagens/foto'+i`.

## Hospedar no GitHub Pages

1. Crie um repositório **público** no GitHub.
2. **Add file → Upload files**: suba o `index.html` e as fotos.
3. **Settings → Pages → Source**: `Deploy from a branch` → `main` → `/ (root)` → **Save**.
4. Em ~1 min o link aparece: `https://seuusuario.github.io/nome-do-repo/`.

Dica: repositório nomeado exatamente como `seuusuario.github.io` dá link limpo sem o nome do repo no fim.

## Adicionar fotos

Numere em sequência a partir de 1, **sem pular números**: `foto1.jpg`, `foto2.jpg`, `foto3.jpg`…
Formatos: `.jpg`, `.jpeg`, `.png`, `.webp`. Carrossel sem limite, com setas, bolinhas, swipe no celular e autoplay.

**Comprima as fotos** antes de subir ([squoosh.app](https://squoosh.app/)). Muitas fotos pesadas deixam o site lento.

## Trocar a música

No `index.html` procure por `0tgVpDi06FyKpA1z0VMD4v` (ID da música no Spotify — hoje "Perfect", Ed Sheeran).
No Spotify: três pontinhos → Compartilhar → Copiar link → pegue o trecho depois de `/track/` e antes do `?` e substitua.

## Trocar as datas

No `index.html`:
```js
var events = {
  kiss:   new Date(2012, 9, 15, 21, 0, 0),  // 15/out/2012 21h
  namoro: new Date(2013, 4, 1, 20, 0, 0)    // 01/mai/2013 20h
};
```
**Mês é zero-indexado**: janeiro = 0 … dezembro = 11. Lembre de trocar também os textos das datas logo acima dos cronômetros.

## Mudar o tema padrão

Na tag `<body class="theme-classic">`, troque por `theme-polaroid`, `theme-night` ou `theme-garden`.
