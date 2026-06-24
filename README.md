# Utilização do Sistema

## Instalação das dependências

Antes de tudo, certifique-se de que o node.js e o npm estão instalados de forma correta em sua máquina, caso não esteja, acesse o site do node.js e faça a instalação:
[https://nodejs.org/pt-br](https://nodejs.org/pt-br)

depois, baixe os arquivos do respositório em sua máquina e abra a pasta onde todos os arquivos se encontram no terminal ou no prompt de comandos e realize a instalação das depêndencias do projeto utilizando um dos seguintes comandos:

```npm i --save``` ou ```npm install --save```

## Configurações do bot:

Acesse o site de desenvolvedores do Discord, crie uma nova aplicação e resgate as seguintes informações:
`Client_ID` && `Token`

Após isso, obtenha o ID referente ao cargo que deseja adicionar e o servidor que vai ser afetado pela aplicação.
Com todas as informações coletadas, abra o código do arquivo `index.js` no seu VS Code ou no bloco de notas e substitua as seguintes linhas com as informações obtidas anteriormente:

TOKEN : `client.login('Seu Token Aqui');`, na ultima linha do código `52`

ID do Servidor : `const GUILD_ID = 'Id do servidor';` na linha `9`

ID do Cargo : `const ROLE_ID = 'Id do cargo que será adicionado';` na linha `10`

## Execução da aplicação:

Depois de tudo configurado corretamente basta, no mesmo terminal/cmd onde instalou as depêndencias do projeto, execute o seguinte comando:

```node .``` ou ```node index.js```

O código irá começar a ser executado e os membros do seu servidor vão receber o cargo um por um. Em servidores com muitos membros, pode demorar um pouco, já que ele adiciona o cargo em um membro a cada 1 segundo, para evitar que o código quebre no meio do processo por muitas requisições simultâneas.

Basta acompanhar os logs no proprio terminal para saber quais membros receberam o cargo, quantos faltam e quando a aplicação terminar sua execução.

## Imagem demonstrativa:

<img width="1113" height="618" alt="image" src="https://github.com/user-attachments/assets/5162131a-2b2a-4c5f-96f2-0a9c428169ac" />
