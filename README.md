# Site oficial da RDTech

Site institucional estático para `rdtech.dev.br`, preparado para deploy na Vercel e para verificação de propriedade no Google Search Console antes da validação da organização no Google Play Console.

## Estrutura

- `index.html`: página principal da RDTech.
- `produtos/carro-das-delicias/index.html`: página pública do aplicativo Carro das Delícias como produto da RDTech.
- `contato/index.html`: canal oficial de contato.
- `privacidade/index.html`: política de privacidade institucional.
- `termos/index.html`: termos de uso do site.
- `robots.txt` e `sitemap.xml`: indexação.
- `.well-known/security.txt`: contato público para assuntos de segurança.
- `assets/rdtech-technology-workspace.webp`: imagem principal otimizada para carregamento rápido, com PNG como fallback.
- `assets/rdtech-icon.png`: ícone oficial da empresa, gerado a partir da imagem do perfil RD Tech.
- `assets/carro-das-delicias-icon.png`: ícone oficial do aplicativo Carro das Delícias usado na página do produto.
- `vercel.json`: URLs limpas, barras finais e headers básicos de segurança.

## Deploy na Vercel

1. Importe este projeto na Vercel.
2. Configure o domínio `rdtech.dev.br` no projeto.
3. Configure também `www.rdtech.dev.br`, se quiser aceitar o subdomínio `www`.
4. Use os registros DNS exibidos pela própria Vercel no painel do domínio.
5. Aguarde a propagação e confirme que `https://rdtech.dev.br/` abre com HTTPS.

Este projeto não depende de build. A Vercel deve servir os arquivos estáticos diretamente.

## Verificacao no Google Search Console

Recomendado:

1. Abra o Google Search Console.
2. Adicione uma propriedade do tipo **Domínio** para `rdtech.dev.br`.
3. Copie o registro TXT que o Google gerar.
4. Adicione esse TXT no DNS do domínio, no mesmo provedor onde você configura os apontamentos para a Vercel.
5. Aguarde a propagação e clique em **Verificar** no Search Console.

Alternativa:

- Se preferir uma propriedade de **prefixo de URL**, use `https://rdtech.dev.br/`.
- O Google pode oferecer uma meta tag HTML. Nesse caso, cole a tag exata no `<head>` de `index.html`, no ponto marcado pelo comentário de Search Console.

## Validacao no Google Play Console

Depois que o domínio estiver verificado no Search Console:

1. No Play Console, abra **Detalhes da conta**.
2. Informe `https://rdtech.dev.br/` como site principal da organização.
3. Envie o pedido de verificação.
4. Aprove a solicitação no Search Console com o mesmo usuário proprietário da propriedade.

## Ajustes antes de publicar

- O único e-mail público configurado no site é `suporte@rdtech.dev.br`.
- Se a conta de desenvolvedor do Google Play usa razão social, CNPJ ou endereço comercial específico, atualize o bloco "Informações institucionais" com os dados oficiais correspondentes.
- Aplicativos publicados pela RDTech podem ter páginas próprias dentro de `produtos/` e documentos específicos no site público de cada app.
