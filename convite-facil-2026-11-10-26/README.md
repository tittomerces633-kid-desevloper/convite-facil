# Convite Fácil 💌

Aplicativo estático e responsivo para criar convites digitais. Pode ser publicado na Vercel ou no GitHub Pages sem etapa de build.

## Recursos

- Vitrine de modelos por categoria e editor com prévia ao vivo.
- Criar, editar, excluir, buscar, baixar e compartilhar convites.
- Campo opcional de e-mail do participante, mostrado no painel administrativo local.
- Login demonstrativo do participante por e-mail e filtro de convites associados a esse e-mail no navegador atual.
- O e-mail do participante não é incluído no link público compartilhado do convite.
- Painel administrativo com dashboard, status, modelos, notificações locais, configurações e registros.
- Layout responsivo para celular, tablet e computador.

## Publicar na Vercel

1. Entre em https://vercel.com e crie/importa um projeto.
2. Envie os arquivos da raiz do ZIP ou conecte um repositório GitHub que contenha `index.html`.
3. Para esta versão estática, não é necessário comando de build; a raiz do projeto contém o `index.html`.

## Publicar no GitHub Pages

1. Envie `index.html`, `README.md` e `LICENSE` para a raiz do repositório.
2. Abra **Settings → Pages**, selecione **Deploy from a branch**, branch `main`, pasta `/(root)`, e salve.

## Importante sobre dados e segurança

Esta versão não possui servidor nem banco de dados. Convites e registros ficam apenas no navegador/dispositivo atual, sem sincronização entre usuários. O e-mail do participante fica armazenado no `localStorage` local e não vai no link público do convite. O login do participante é somente uma identificação local por e-mail: não utiliza senha, não verifica a identidade em um servidor e não protege dados reais. Para sincronizar dados entre participantes ou gerenciar dados reais, conecte uma API, banco de dados e autenticação segura no servidor.

O login administrativo da versão atual é uma checagem no JavaScript do navegador e **não protege um site público**: as credenciais podem ser encontradas no código. Não use credenciais reais nesta versão nem publique uma senha pessoal em repositório público.

## Arquivos

- `index.html`: aplicativo inteiro (HTML, CSS e JavaScript).
- `README.md`: instruções.
- `LICENSE`: licença MIT.
