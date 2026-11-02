# Rotina Diária

App web instalável (PWA). Funciona offline e os dados ficam no telemóvel (localStorage do Chrome).

## Pôr online (uma vez) com GitHub Pages
1. Cria um repositório no GitHub (pode ser privado só com GitHub Pro; público funciona sempre — os teus dados não vão para lá, só o código).
2. Envia estes ficheiros para a raiz do repositório.
3. Settings → Pages → Source: "Deploy from a branch" → `main` / `(root)`.
4. Fica em `https://<utilizador>.github.io/<repo>/`.

Alternativas iguais: Netlify Drop (arrasta a pasta), Cloudflare Pages. Precisa de HTTPS para o modo offline.

## Instalar no Android
1. Abre o endereço no Chrome.
2. Menu ⋮ → "Adicionar ao ecrã principal" → "Instalar".
3. A partir daí abre como app, sem barra do browser, e funciona sem rede.

## Dados
- Ficam só no telemóvel, dentro do Chrome. Desinstalar a app ou limpar os dados do Chrome apaga-os.
- Em Ajustes → Cópia de segurança: exporta um JSON de vez em quando. Importar repõe tudo.

## Actualizar a app
Altera `index.html`, sobe a versão em `sw.js` (`rotina-v2`, …) e faz push. A app apanha a nova versão na abertura seguinte com rede.
