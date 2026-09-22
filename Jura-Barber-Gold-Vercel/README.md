# Jura Barber Gold — landing page

Projeto estático pronto para editar no VS Code e publicar na Vercel. Não precisa instalar dependências nem executar build.

## Arquivos

- `index.html` — página completa, incluindo estilos, animações, textos e scripts.
- `assets/logo.png` — logo fornecida para a página.
- `assets/videos/` — coloque aqui os vídeos quando estiverem prontos.

## Abrir e editar

Abra esta pasta no VS Code. Para conferir, abra `index.html` no navegador. Para ter recarregamento automático durante a edição, você também pode usar uma extensão de servidor local no VS Code.

As partes mais fáceis de alterar estão no próprio `index.html`: serviços na seção `id="servicos"`, textos nas seções correspondentes, cores no bloco `:root` do CSS e telefone em `WHATSAPP_NUMBER` no script ao final do arquivo.

## Adicionar os quatro vídeos

1. Copie os arquivos para `assets/videos/`. Sugestão: `vertical-1.mp4`, `vertical-2.mp4`, `horizontal-1.mp4` e `horizontal-2.mp4`.
2. No final do `index.html`, procure `const VIDEO_FILES` e preencha os caminhos:

```js
const VIDEO_FILES = {
  vertical1: 'assets/videos/vertical-1.mp4',
  vertical2: 'assets/videos/vertical-2.mp4',
  horizontal1: 'assets/videos/horizontal-1.mp4',
  horizontal2: 'assets/videos/horizontal-2.mp4'
};
```

As **quatro molduras já aparecem na página**: duas verticais no início e duas horizontais perto do fim. Ao preencher um caminho, o vídeo substitui a arte naquela moldura. Se o caminho estiver vazio ou o arquivo não carregar, a arte da Jura continua visível. Os verticais começam sem som e em repetição; todos exibem controles. Recomenda-se MP4 com codec H.264 para boa compatibilidade. Comprima os vídeos antes de publicar para melhorar o carregamento.

## Publicar na Vercel

Envie esta pasta como projeto estático, mantendo `index.html` na raiz. Você pode usar o [Vercel Drop](https://vercel.com/drop) para arrastar a pasta descompactada ou importar um repositório Git. Na importação, selecione **Other** como Framework Preset, deixe o Build Command vazio e sirva a raiz (`.`). Não há pasta `dist`.

O WhatsApp de agendamento já aponta para `+55 21 96650-8588`. O site não cobra, confirma nem registra horários por conta própria: o atendimento continua pelo WhatsApp.
