Anotações sobre a API

Neste arquivo será documentado os comandos utilizados no terminal e acriação de pastas. Em relação as alterações no código, as anotações estarão no mesmo (menos em arquivo json, já que comentários não são suportados)


COMANDOS NO TERMINAL

    **npm init -y**
        Esse comando é para configuração do ambiente. Após faze-lo é criado um arquivo json que contem todas as informações sobre o projeto (packpage.json)

    **npm install express mysql dotenv cors body-parser**
        Este comando é para a instalção de dependências para o nosso projeto. Essas dependências estão sendo puxadas pelo express

    **npm nodemon --save-dev**
        Este comando é para instalar o nodemon porém está indicando aqui que ele será instalado em abiente de desenvolvimento. Uma diferença visível de quando instala padrão é que com o --save-dev ele deixa salvo no arquivo json como "devDependencies", e não junto com os outros. 

    -> Quando salvar em um ambiente de desenvolvimento?
        O **--save-dev**('devdependencies') é usado quando o pacote é necessário apenas durante o desenvolvimento ou para tarefas de construção(como por exemplo testes, compilação de código, linting). 

            Exemplos de pacotes utilizados: 
            Ferramentas testes - Mocha, Jest;
            Ferramentas de empacotamento -  Webpack, Gulp;
            Utilitárias de desenvolvimento - Nodemon, ESlint.
        O **--save** ('dependencies') é usado quando o pacote é necessário para o aplivativo em si, ou seja, para sua execução em produção. Eles podem ser bibliotecas ou frameworks.

        Também tem a opção de **não especificar nenhum**, que geralmente é feito quando você deseja instalar um pacote globalmente, ou seja, disponível em todo o sistema.

CRIANDO ARQUIVOS...

    **src**: É uma abreviação de "source". É uma maneira de organizar o código-fonte do projeto. Muito útil em projetos grandes. Também é bom para melhorar a modularização do aplicativo e facilitar a manutenção do código. Também é uma boa prática por melhorar a legibilidade da estrutura de diretórios. 
    **variaveis.env**: É um arquivo de configuração. Usaremos o arquivo pra armarzenar configurações do sistema e variáveis como por exemplo uma porta de conexão nossa com o servidor, nosso string de conexão com o banco de dados, usuário, senha... 

ALTERAÇÕES NO ARQUIVO JSON





