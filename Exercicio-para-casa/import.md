# Sistema Windows

→  **para importar o arquivo herois**

Se estiver usando a versão 4.4 do MongoDB  você vai precisar instalar o MongoDB database Tools!

→ Importanto o arquivo :  na pasta **C:\Program Files\MongoDB\Tools\100\bin**  coloque o arquivo herois.json 

→ Abra um novo CMD no endereço desta pasta

→ execute o comando:

 mongoimport --db reprograma --collection “nomeDaCollection” --jsonArray --file herois.json


vai ficar assim

![imagem](./img/01.jpg)


→ no endereço C:\Program Files\MongoDB\Server\4.4\bin  clicar duas vezes  em mongod , ele vai mostrar um monte de código.

→ No endereço  C:\Program Files\MongoDB\Server\4.4\bin
escrever cmd e aperte enter, ele vai abrir o prompt dentro dessa pasta

→ executar mongo.exe no prompt

//O comando mongod faz com o que processo do banco de dados inicie.
//O comando mongo faz com que você se conecte com uma instância específica do mongo

→ show dbs  -- Vai mostrar o que tem de banco de dados
// (por padrão mostra esses dois, mas se vc tiver mais na máquina ele vai mostrar os outros também) 

admin      0.000GB
config      0.000GB
reprograma     0.000GB

→ digite o comando use reprograma
→ digite o comando show collections

E lá vai estar o seu arquivo importado! 

![imagem](./img/02.jpg)

