## Passo a Passo para Rodar a Aplicação Localmente

Clone o repositório do projeto para o seu sistema local:

    git clone <URL_do_Repositório>

Navegue até o diretório do projeto:

    cd <Nome_do_Diretório_do_Projeto>

Crie as imagens e os conteineres

    docker compose -f docker-compose.yml up

## Navegando Pelo Seu Navegador do Browser

Digite o seguinte URL na barra de endereços:

    http://localhost:8080

A aplicação deve ser carregada e você poderá interagir com ela através do navegador.

Certifique-se de que a porta 8080 seja a porta correta em que a aplicação está sendo executada. Se a aplicação estiver configurada para usar uma porta diferente, substitua 8080 pelo número da porta correto.

## Testando Seu Projeto

Senha para acessar sua conta:

    usuário: admin_vp
    senha: admin_vp

Ao logar faça os seguintes testes, para ter certeza que os conteineres estão se comunicando e funcionando:

    - Clique em ALL USERS, depois escolha um dos user ID, ao clicar uma mensagem pedindo para retornar aparecerá, clique em BACK e clique novamente no mesmo ID. Se você recebeu uma mensagem com novos dados, o banco de dados está funcionando.

Retorne para sua conta de login
    - Clique em RABBITMQ, se a mensagem "Generated 2 Connections 6; Chanels 1 Exchage and 2 Que" apareceu em sua tela, o mesmo está em correto funcionamento.


