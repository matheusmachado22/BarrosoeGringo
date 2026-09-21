# Barroso & Gringo

Site institucional estático para escritório de advocacia.

## Publicar na Vercel

1. Instale o Node.js apenas se quiser usar a CLI; para este site não é obrigatório.
2. Crie um repositório no GitHub e envie os arquivos desta pasta.
3. Em [vercel.com](https://vercel.com), selecione **Add New > Project**, importe o repositório e clique em **Deploy**.
4. Não defina build command nem output directory: a raiz do projeto já contém o `index.html`.

## Ligar o domínio da GoDaddy

1. Na Vercel, abra o projeto em **Settings > Domains**, adicione `seudominio.com.br` e `www.seudominio.com.br`.
2. Na GoDaddy, abra **DNS Management** e crie/ajuste:
   - `A` para `@` apontando para `76.76.21.21`.
   - `CNAME` para `www` apontando para `cname.vercel-dns.com`.
3. Remova registros conflitantes de `@` e `www`. A propagação pode levar algumas horas.
4. Volte à Vercel e aguarde o domínio aparecer como verificado. O HTTPS será provisionado automaticamente.

Antes de publicar, substitua o e-mail e telefone de exemplo no `index.html`.
