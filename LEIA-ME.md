# Publis em Dia 🎀

Aplicativo web responsivo para organizar publis, valores e pagamentos.

## Arquivos
- `index.html`: aplicativo completo.
- `manifest.json`: configuração para instalação como app.
- `sw.js`: cache básico para abrir mais rápido e permitir uso offline após a primeira visita.
- `icon.svg`: ícone do aplicativo.

## Publicar gratuitamente pelo iPhone com GitHub Pages
1. No Safari, entre em https://github.com e crie uma conta ou entre na sua conta.
2. Toque no `+` e escolha **New repository**.
3. Dê o nome `publis-em-dia`, marque **Public** e toque em **Create repository**.
4. Dentro do repositório, use **Add file** → **Upload files**. Envie os quatro arquivos deste pacote (`index.html`, `manifest.json`, `sw.js`, `icon.svg`). Se o GitHub móvel não mostrar essa opção, abra o menu do Safari `aA` → **Solicitar Site para Computador** e tente novamente.
5. Toque em **Commit changes** para salvar os arquivos.
6. No repositório, abra **Settings** → **Pages**. Em **Build and deployment**, escolha **Deploy from a branch**; selecione `main` e `/ (root)`; toque em **Save**.
7. Aguarde a publicação. O endereço costuma ser `https://SEU-USUARIO.github.io/publis-em-dia/`. Não considere publicado até abrir esse endereço no Safari e ver a tela do app funcionando. O primeiro deploy pode levar alguns minutos.
8. Para instalar no iPhone: abra o link no **Safari** → botão **Compartilhar** → **Adicionar à Tela de Início** → ative **Abrir como App** se aparecer → **Adicionar**.

## Salvar e recuperar dados
Os registros ficam no armazenamento local do navegador (`localStorage`) do aparelho. Eles não são enviados para um servidor e não sincronizam automaticamente entre dispositivos. Não limpe os dados do Safari sem antes exportar um backup. Use ⚙ → **Exportar backup** para baixar um arquivo JSON; guarde-o no app Arquivos/iCloud Drive. Para recuperar, abra ⚙ → **Restaurar backup** e escolha o arquivo JSON. A restauração substitui os registros existentes.

## Limites importantes
- Este projeto não tem conta de usuário nem sincronização em nuvem. Para um controle financeiro com sincronização entre aparelhos, seria necessário configurar um serviço de banco de dados/autenticação, como Supabase, e adaptar o app.
- O app é uma ferramenta de organização, não um sistema contábil ou fiscal.
- O link de hospedagem só passa a existir depois de publicar no GitHub Pages; este pacote não foi publicado automaticamente.
