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

    **routes.js**:São as rotas e caminhos que estão dentro da API. Quando formos configurar o CRUD (Create, Read, update, delete) vamos ter caminhos para criar, ler, alterar e deletar.

    **server.js**: 'dotenv' ajuda a ler o arquivo de variável de ambiente (aqui no caso variaveis.env). Então colocamos ele como parâmetro usando o path.
        cors: Permite acesso pra trabalhar com recursos de outros site mesmo estando em dominios diferentes.
        linha "const routes = require('./routes') " é onde mostra onde estará a rota

    **packpage.json**(gerado por comando no terminal): É um arquivo utilizado em projetos Node.js para descrever o próprio projeto, incluindo metadados como nome, versão, descrição, scripts de inicialização, testes, entre outros. Além disso, o package.json é usado para listar as dependências do projeto, ou seja, os pacotes que o projeto utiliza. Isso permite que outros desenvolvedores possam facilmente instalar as mesmas dependências e executar o projeto em seus próprios ambientes de desenvolvimento.

    **packpage-lock.json**(gerado por comando no terminal):um arquivo gerado automaticamente que registra as versões exatas de todas as dependências do seu projeto. Ele garante que, ao instalar as dependências em outro ambiente, as mesmas versões serão instaladas, evitando inconsistências e garantindo a reprodução consistente do ambiente de desenvolvimento.


EXPLICANDO PÁGINAS...
    routes: Fazendo uma requisição e chamando o express.Quando essa rota for executada de alguma maneira iremos chama-la e exporta-la. 


