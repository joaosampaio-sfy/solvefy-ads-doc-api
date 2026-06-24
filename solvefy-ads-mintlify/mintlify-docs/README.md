# Solvefy Ads — Documentação API (Mintlify)

Documentação oficial da API Solvefy Ads, pronta para publicar no Mintlify.

## Estrutura de arquivos

```
mintlify-docs/
├── mint.json                          ← configuração principal
├── favicon.svg
├── logo/
│   ├── logo-dark.svg
│   └── logo-light.svg
├── introducao.mdx
├── autenticacao.mdx
├── erros.mdx
└── api-reference/
    ├── usuarios/
    │   ├── me.mdx
    │   ├── criar.mdx
    │   ├── atualizar.mdx
    │   └── remover.mdx
    ├── subcontas/
    │   ├── me.mdx
    │   ├── criar.mdx
    │   ├── atualizar.mdx
    │   └── remover.mdx
    ├── campanhas/
    │   └── visao-geral.mdx
    ├── billing/
    │   └── recarga.mdx
    └── webhooks/
        ├── registrar.mdx
        └── atualizar.mdx
```

## Como publicar

### 1. Criar repositório no GitHub

1. Crie um repositório público (ou privado) no GitHub — ex.: `solvefy-ads-docs`
2. Suba todos estes arquivos para a branch `main`

```bash
git init
git add .
git commit -m "feat: documentação inicial API Solvefy Ads"
git remote add origin https://github.com/SEU_ORG/solvefy-ads-docs.git
git push -u origin main
```

### 2. Conectar ao Mintlify

1. Acesse **[dashboard.mintlify.com](https://dashboard.mintlify.com)**
2. Clique em **New Project**
3. Conecte sua conta do GitHub e selecione o repositório
4. O Mintlify detecta o `mint.json` automaticamente e faz o deploy

### 3. Domínio personalizado (opcional)

No painel do Mintlify, vá em **Settings → Custom Domain** e configure:

```
docs.solvefy.com  →  CNAME  →  solvefy-ads-docs.mintlify.app
```

### 4. Atualizações futuras

Qualquer push na branch `main` faz o redeploy automático.

---

## Configurações em mint.json

Para atualizar cor, logo ou links, edite o `mint.json`.

- `colors.primary` → cor de destaque (atualmente laranja `#F5A623`)
- `topbarCtaButton` → botão de destaque no topo
- `navigation` → estrutura do menu lateral
