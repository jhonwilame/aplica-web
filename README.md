# Página de Login Interativa com HTML, CSS, Docker e AWS EC2

Este projeto consiste em uma página de login interativa desenvolvida com HTML e CSS, com o objetivo de servir como ambiente de aprendizado e experimentação. A aplicação foi implantada em uma instância EC2 da AWS, utilizando Docker para containerização e Apache como servidor web.

## Tecnologias

*   **Front-end:** HTML e CSS
*   **Back-end:** (Em desenvolvimento)
*   **Infraestrutura:**
    *   AWS EC2 (Amazon Linux 2)
    *   Docker
    *   Apache

## Funcionalidades

*   Página de login com design responsivo e interface amigável.
*   Implantação em ambiente AWS EC2.
*   Containerização com Docker para portabilidade e escalabilidade.

## Arquitetura

1.  **Desenvolvimento:** A página de login foi desenvolvida utilizando HTML para a estrutura e CSS para o design.
2.  **Implantação:**
    *   Uma instância EC2 com Amazon Linux 2 foi provisionada na AWS.
    *   Docker e Git foram instalados na instância EC2.
    *   O repositório do projeto foi clonado do GitHub.
    *   Uma imagem Docker foi construída utilizando uma imagem base do Apache, copiando os arquivos da aplicação para o diretório de arquivos estáticos do Apache.
    *   Um container Docker foi executado, com a porta 80 do container mapeada para a porta 80 da instância EC2.

## Como executar

1.  Clone o repositório:

    ```bash
    git clone [https://github.com/seu-usuario/seu-repositorio.git](https://www.google.com/search?q=https://github.com/seu-usuario/seu-repositorio.git)
    ```

2.  Navegue até o diretório do projeto:

    ```bash
    cd seu-repositorio
    ```

3.  Construa a imagem Docker:

    ```bash
    docker build -t meu-app .
    ```

4.  Execute o container Docker:

    ```bash
    docker run -d -p 80:80 meu-app
    ```

5.  Acesse a aplicação no seu navegador:

    ```
    http://<endereço-ip-da-sua-instancia-ec2>
    ```

## Próximos passos

*   Implementar autenticação de usuários.
*   Integrar com um banco de dados.
*   Adicionar testes automatizados.
*   Configurar deploy contínuo.

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e enviar pull requests.



