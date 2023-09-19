# S2-02A-Node.js

Esse é um código para uma tarefa envolvendo a criação de um servidor Node.js
Para realizar a ativação do Node.js, siga os passos abaixo (o tutorial será em linhas de comando para o terminal do Linux):

### Instalar o Node.js
1. Primeiro, você precisa ter o python3-pip instalado na sua máquina. Você pode fazer isso digitando `sudo apt install python3-pip` no terminal do Linux.
2. Depois, com o pip3 instale o Nodeenv com o comando `pip3 install --user nodeenv`.
3. Agora reinicie a máquina ou digite o comando `pip3 install --user nodeenv`, e para testar digite `nodeenv --version` que deve retornar a versão do Nodeenv que foi instalada.
4. Finalmente, para instalar o Node.js digite `nodeenv [nome da pasta do Node.js]`, e caso queira testar, o comando `node --version` deve retornar a versão do Node.js que foi instalada.
5. Para ativá-lo use `source ./[pasta do Node.js]/bin/activate` e `deactivate_node` para desativá-lo.

### Criando o servidor Node.js
1. Antes de tudo, se certifique de estar com o Node desativado.
2. Vá para a pasta que você criou ao instalar o Node.js e crie um arquivo com extensão .js (para essa atividade, criei um arquivo com o nome de index.js).
3. Abra esse arquivo para editar seu conteúdo e digite o seguinte código:
`var http = require('http');

http.createServer(function (req, res) {
  res.writeHead(200, {'Content-Type': 'text/plain'});
  res.end('Adrielly Souza Inocencio - 19/09/2023');
}).listen(8013);`
3. Salve o arquivo e ative o Node.
4. Por fim, digite o seguinte endereço em um navegador: localhost:8013
