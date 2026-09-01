# VARISPEED — site de apresentação

Site de apresentação independente do
[nehalem-x/VARISPEED](https://github.com/nehalem-x/VARISPEED). Ele pode ser
clonado separadamente ou mantido na pasta `website/` do projeto principal. O
repositório não possui configuração de publicação e, por padrão, funciona
localmente.

## Desenvolvimento

```bash
npm ci
npm run dev
```

Abra o endereço local exibido pelo servidor de desenvolvimento (normalmente
`http://localhost:3000`).

Verificações de qualidade:

```bash
npm run lint
npx tsc --noEmit
npm run build
npm audit --omit=dev
```

O grafo interativo reutiliza o `GraphEngine` de produção do VARISPEED. O campo
de partículas da seção principal usa um shader local em Three.js e respeita as
preferências de movimento reduzido e de visibilidade da página.

![Visão geral do site de apresentação do VARISPEED](./docs/varispeed-site-preview-2026-08-31.png)
