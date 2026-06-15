# Meu Treino

App (PWA) de registro de treinos de musculação. Funciona offline e instala na tela inicial do celular.

## Como funciona
- Os dados ficam **no próprio aparelho** (`localStorage`) — não há servidor nem conta.
- Use o botão **⬇︎ Backup** para salvar uma cópia (JSON) e o **⬆︎** para restaurar.

## Atualizar o app
Ao mudar qualquer arquivo, suba o número da versão em `sw.js` (`meu-treino-v1` → `v2`)
para o celular baixar a nova versão. Depois faça commit e `git push`.

## Estrutura
- `index.html` — app inteiro (UI + lógica)
- `chart.umd.min.js` — Chart.js embutido (gráficos offline)
- `sw.js` — service worker (cache offline)
- `manifest.webmanifest` + `icon-*.png` / `apple-touch-icon.png` — instalação na tela inicial
