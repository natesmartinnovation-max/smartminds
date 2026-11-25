# Smart Minds · site (protótipo)

Site one page estático (HTML/CSS/JS puro, sem build).

## Publicar na Vercel
1. Crie um repositório no GitHub e envie o conteúdo desta pasta (ou use `vercel` na CLI dentro dela).
2. Na Vercel: **Add New → Project → Import** o repositório.
3. Framework Preset: **Other**. Build Command: vazio. Output Directory: `.` (raiz).
4. Deploy. Depois, em **Settings → Domains**, adicione `smartminds.ia.br` e siga as instruções de DNS do Registro.br.

## Arquivos
- `index.html`: página principal
- `404.html`: página de erro (a Vercel usa automaticamente)
- `og.jpg`: cartão de compartilhamento (WhatsApp, LinkedIn, etc.) 1200×630
- `favicon.ico`, `favicon.svg`, `apple-touch-icon.png`, `icon-192.png`, `icon-512.png`, `site.webmanifest`: ícones
- `robots.txt`, `sitemap.xml`: indexação
- `vercel.json`: URLs limpas, cache de imagens e cabeçalhos de segurança

## Antes de ir ao ar
- As URLs de compartilhamento apontam para `https://smartminds.ia.br`. Se publicar antes em outro domínio (ex.: `*.vercel.app`), troque esse endereço no `<head>` do `index.html` para o preview do WhatsApp funcionar.
- O formulário de contato e a newsletter ainda não enviam dados. Para ativar, conecte a um serviço como Formspree, Resend ou uma Vercel Function.
- O WhatsApp guarda o preview em cache: depois de publicar, teste o link no Facebook Sharing Debugger para forçar a atualização.
