# Site da ATF Consulting

Site institucional de página única da ATF Consulting, feito em HTML e CSS. Não precisa de instalação nem de servidor próprio e pode ser publicado de graça no GitHub Pages.

## O que tem nesta pasta

| Arquivo | Para que serve |
|---|---|
| `index.html` | O site completo, com textos, estilos e funcionamento. |
| `404.html` | A página exibida quando alguém acessa um endereço que não existe. |
| `assets/logo-atf.png` | O logo original da ATF, com fundo transparente. |
| `favicon.ico`, `favicon.png`, `apple-touch-icon.png`, `icon-512.png` | Os ícones da aba do navegador e da tela inicial do celular. |
| `og-image.jpg` | A imagem que aparece quando o link do site é compartilhado no WhatsApp e em outras redes. |
| `robots.txt`, `sitemap.xml` | Os arquivos que ajudam o Google a encontrar e indexar o site. |

## Como publicar no GitHub Pages

1. **Crie o repositório.** Entre no GitHub, clique em **New repository** e dê um nome, por exemplo `atf-site`. Deixe o repositório como **Public**: no plano gratuito, o GitHub Pages só funciona com repositório público.
2. **Envie os arquivos.** No repositório, vá em **Add file → Upload files** e arraste todo o conteúdo desta pasta, incluindo a pasta `assets`. Depois clique em **Commit changes**.
3. **Ative o GitHub Pages.** Vá em **Settings → Pages**. Em **Build and deployment**, escolha **Deploy from a branch**, depois a branch `main` e a pasta `/ (root)`, e clique em **Save**.
4. **Acesse o site.** Em poucos minutos, o site fica disponível em `https://SEU-USUARIO.github.io/atf-site/`.

## Como usar o domínio atfconsulting.com.br (opcional)

1. No GitHub, vá em **Settings → Pages → Custom domain**, digite `atfconsulting.com.br` e clique em **Save**.
2. No painel onde o domínio está registrado (por exemplo, o Registro.br), abra a configuração de DNS e crie estes registros:
   - Quatro registros do tipo **A** para `atfconsulting.com.br`, apontando para `185.199.108.153`, `185.199.109.153`, `185.199.110.153` e `185.199.111.153`.
   - Um registro do tipo **CNAME** para `www`, apontando para `SEU-USUARIO.github.io`.
3. **Não altere nem apague os registros MX nem os outros registros do e-mail.** São eles que fazem o `contato@atfconsulting.com.br` funcionar.
4. Quando o GitHub confirmar o domínio, o que pode levar algumas horas, marque **Enforce HTTPS**.

O site já aponta para `https://atfconsulting.com.br/` no link canônico, na imagem de compartilhamento e no `sitemap.xml`. Se for usar outro endereço, troque esse endereço no `index.html`, no `robots.txt` e no `sitemap.xml`.

## Como alterar contatos e textos

Abra o `index.html` em qualquer editor de texto, ou direto no GitHub pelo ícone de lápis, e use a busca para encontrar o que quer trocar:

- **Telefones e WhatsApp:** o site usa dois números. Procure `95407-0048` e `5511954070048` para o (11) 95407-0048, e `98828-2200` e `5527988282200` para o (27) 98828-2200. Os números longos são os usados nos links do WhatsApp e de ligação, no formato 55 + DDD + número. Os botões principais e o botão flutuante do WhatsApp usam o (11).
- **E-mail:** procure `contato@atfconsulting.com.br`.
- **Endereço:** procure `Av. Tupã`.
- **Instagram:** procure `atf.consulting`.

O formulário de contato não guarda dados. Ele só monta a mensagem e a abre no WhatsApp ou no e-mail de quem está preenchendo.
