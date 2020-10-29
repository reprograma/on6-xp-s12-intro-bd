# Desafio semana 12

**Você receberá um arquivo com o formato JSON contendo alguns personagens de quadrinhos e/ou desenhos animados e você deverá realizar as alterações que foram solicitadas abaixo pelo cliente.**

**1**.Selecione todos os registros.

 ```javascript   
db.Hdeherois.find()

//ou 

db.Hdeherois.find().pretty()

    {
            "_id" : ObjectId("5f99cb2cc645577c0a6750bc"),
            "nome" : "Gavião Arqueiro",
            "dateOfBirth" : "1981-03-18T08:30:00.000Z",
            "local" : "Roma",
            "usaCapa" : false,
            "quantidadeGatos" : 1,
            "quantidadeCachorros" : 0
    }
    {
            "_id" : ObjectId("5f99cb2cc645577c0a6750bd"),
            "nome" : "Shrek",
            "dateOfBirth" : "1785-04-06T08:30:00.000Z",
            "local" : "Londres",
            "usaCapa" : false,
            "quantidadeGatos" : 5,
            "quantidadeCachorros" : 2
    }
    {
            "_id" : ObjectId("5f99cb2cc645577c0a6750be"),
            "nome" : "Homem Formiga",
            "dateOfBirth" : "1962-01-27T08:30:00.000Z",
            "local" : "Londres",
            "usaCapa" : false,
            "quantidadeGatos" : 4,
            "quantidadeCachorros" : 5
    }
    {
            "_id" : ObjectId("5f99cb2cc645577c0a6750bf"),
            "nome" : "Batman",
            "dateOfBirth" : "1939-10-01T08:30:00.000Z",
            "local" : "Detroit",
            "usaCapa" : true,
            "quantidadeGatos" : 2,
            "quantidadeCachorros" : 7
    }
    {
            "_id" : ObjectId("5f99cb2cc645577c0a6750c0"),
            "nome" : "Mulher Maravilha",
            "dateOfBirth" : "1941-12-08T08:30:00.000Z",
            "local" : "Themyscira",
            "usaCapa" : false,
            "quantidadeGatos" : 2,
            "quantidadeCachorros" : 7
    }
    {
            "_id" : ObjectId("5f99cb2cc645577c0a6750c1"),
            "nome" : "Deadpool",
            "dateOfBirth" : "1991-04-25T08:30:00.000Z",
            "local" : "Canadá",
            "usaCapa" : false,
            "quantidadeGatos" : 5,
            "quantidadeCachorros" : 3
    }
    {
            "_id" : ObjectId("5f99cb2cc645577c0a6750c2"),
            "nome" : "Homem de Ferro",
            "dateOfBirth" : "1970-05-29T08:30:00.000Z",
            "local" : "Nova York",
            "usaCapa" : false,
            "quantidadeGatos" : 4,
            "quantidadeCachorros" : 1
    }
    {
            "_id" : ObjectId("5f99cb2cc645577c0a6750c3"),
            "nome" : "Capitão América",
            "dateOfBirth" : "1920-07-04T08:30:00.000Z",
            "local" : "América",
            "usaCapa" : false,
            "quantidadeGatos" : 0,
            "quantidadeCachorros" : 9
    }
    {
            "_id" : ObjectId("5f99cb2cc645577c0a6750c4"),
            "nome" : "Visão",
            "dateOfBirth" : "1940-11-17T08:30:00.000Z",
            "local" : "Nova York",
            "usaCapa" : true,
            "quantidadeGatos" : 4,
            "quantidadeCachorros" : 1
    }
    {
            "_id" : ObjectId("5f99cb2cc645577c0a6750c5"),
            "nome" : "Pantera Negra",
            "dateOfBirth" : "1973-11-25T08:30:00.000Z",
            "local" : "Wakanda",
            "usaCapa" : false,
            "quantidadeGatos" : 7,
            "quantidadeCachorros" : 3
    }
    {
            "_id" : ObjectId("5f99cb2cc645577c0a6750c6"),
            "nome" : "Thor",
            "dateOfBirth" : "1940-05-14T08:30:00.000Z",
            "local" : "Noruega",
            "usaCapa" : true,
            "quantidadeGatos" : 5,
            "quantidadeCachorros" : 3
    }
    {
            "_id" : ObjectId("5f99cb2cc645577c0a6750c7"),
            "nome" : "Hulk",
            "dateOfBirth" : "1969-12-18T08:30:00.000Z",
            "local" : "Novo México",
            "usaCapa" : false,
            "quantidadeGatos" : 1,
            "quantidadeCachorros" : 1
    }
    {
            "_id" : ObjectId("5f99cb2cc645577c0a6750c8"),
            "nome" : "Homem Aranha",
            "dateOfBirth" : "2001-08-10T08:30:00.000Z",
            "local" : "San Francisco",
            "usaCapa" : false,
            "quantidadeGatos" : 0,
            "quantidadeCachorros" : 2
    }
    {
            "_id" : ObjectId("5f99cb2cc645577c0a6750c9"),
            "nome" : "Wolverine",
            "dateOfBirth" : "1880-02-17T08:30:00.000Z",
            "local" : "Canadá",
            "usaCapa" : false,
            "quantidadeGatos" : 3,
            "quantidadeCachorros" : 0
    }
```

**2**.Selecione apenas o primeiro registro.

 ```javascript 
db.Hdeherois.findOne()​ 

{
    "_id" : ObjectId("5f99cb2cc645577c0a6750bc"),
    "nome" : "Gavião Arqueiro",
    "dateOfBirth" : "1981-03-18T08:30:00.000Z",
    "local" : "Roma",
    "usaCapa" : false,
    "quantidadeGatos" : 1,
    "quantidadeCachorros" : 0
}
```


**3**.Selecione todos os registros em que o nome seja igual a ‘Sabrina’ ou a quantidade de gatos seja igual a 2.
db.Hdeherois.find({"nome":"Sabrina", "quantidadeGatos": 2}).pretty()
 ```javascript 
// não tem! 
```

**4**.Selecione todos os registros em que o local de nascimento seja igual a Nova York e necessariamente que a quantidade de cachorros seja igual a 1.

 ```javascript 
db.Hdeherois.find({"local":"Nova York", "quantidadeCachorros": 1}).pretty()

{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c2"),
        "nome" : "Homem de Ferro",
        "dateOfBirth" : "1970-05-29T08:30:00.000Z",
        "local" : "Nova York",
        "usaCapa" : false,
        "quantidadeGatos" : 4,
        "quantidadeCachorros" : 1
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c4"),
        "nome" : "Visão",
        "dateOfBirth" : "1940-11-17T08:30:00.000Z",
        "local" : "Nova York",
        "usaCapa" : true,
        "quantidadeGatos" : 4,
        "quantidadeCachorros" : 1
}
```

**5**.Selecione todos os registros em que a quantidade de gatos seja igual a 4 ou a quantidade de cachorros seja igual a 2.

 ```javascript 
db.Hdeherois.find({ $or:  [{ "quantidadeGatos": 4} , { "quantidadeCachorros": 2 }]}).pretty()

{
        "_id" : ObjectId("5f99cb2cc645577c0a6750bd"),
        "nome" : "Shrek",
        "dateOfBirth" : "1785-04-06T08:30:00.000Z",
        "local" : "Londres",
        "usaCapa" : false,
        "quantidadeGatos" : 5,
        "quantidadeCachorros" : 2
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750be"),
        "nome" : "Homem Formiga",
        "dateOfBirth" : "1962-01-27T08:30:00.000Z",
        "local" : "Londres",
        "usaCapa" : false,
        "quantidadeGatos" : 4,
        "quantidadeCachorros" : 5
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c2"),
        "nome" : "Homem de Ferro",
        "dateOfBirth" : "1970-05-29T08:30:00.000Z",
        "local" : "Nova York",
        "usaCapa" : false,
        "quantidadeGatos" : 4,
        "quantidadeCachorros" : 1
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c4"),
        "nome" : "Visão",
        "dateOfBirth" : "1940-11-17T08:30:00.000Z",
        "local" : "Nova York",
        "usaCapa" : true,
        "quantidadeGatos" : 4,
        "quantidadeCachorros" : 1
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c8"),
        "nome" : "Homem Aranha",
        "dateOfBirth" : "2001-08-10T08:30:00.000Z",
        "local" : "San Francisco",
        "usaCapa" : false,
        "quantidadeGatos" : 0,
        "quantidadeCachorros" : 2
}
```

 **6**.Selecione todos os registros em que o nome comece com C.

 ```javascript 
db.Hdeherois.find({ "nome" : /C/ }).pretty()
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c3"),
        "nome" : "Capitão América",
        "dateOfBirth" : "1920-07-04T08:30:00.000Z",
        "local" : "América",
        "usaCapa" : false,
        "quantidadeGatos" : 0,
        "quantidadeCachorros" : 9
}
```

**7**.Selecione todos os registros em que o nome comece com H.

 ```javascript 
db.Hdeherois.find({ "nome" : /H/ }).pretty()

{
        "_id" : ObjectId("5f99cb2cc645577c0a6750be"),
        "nome" : "Homem Formiga",
        "dateOfBirth" : "1962-01-27T08:30:00.000Z",
        "local" : "Londres",
        "usaCapa" : false,
        "quantidadeGatos" : 4,
        "quantidadeCachorros" : 5
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c2"),
        "nome" : "Homem de Ferro",
        "dateOfBirth" : "1970-05-29T08:30:00.000Z",
        "local" : "Nova York",
        "usaCapa" : false,
        "quantidadeGatos" : 4,
        "quantidadeCachorros" : 1
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c7"),
        "nome" : "Hulk",
        "dateOfBirth" : "1969-12-18T08:30:00.000Z",
        "local" : "Novo México",
        "usaCapa" : false,
        "quantidadeGatos" : 1,
        "quantidadeCachorros" : 1
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c8"),
        "nome" : "Homem Aranha",
        "dateOfBirth" : "2001-08-10T08:30:00.000Z",
        "local" : "San Francisco",
        "usaCapa" : false,
        "quantidadeGatos" : 0,
        "quantidadeCachorros" : 2
}
```

**8**.Selecione todos os registros em que o nome termine com a.

 ```javascript 
db.Hdeherois.find({ "nome" : /a$/ }).pretty()
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750be"),
        "nome" : "Homem Formiga",
        "dateOfBirth" : "1962-01-27T08:30:00.000Z",
        "local" : "Londres",
        "usaCapa" : false,
        "quantidadeGatos" : 4,
        "quantidadeCachorros" : 5
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c0"),
        "nome" : "Mulher Maravilha",
        "dateOfBirth" : "1941-12-08T08:30:00.000Z",
        "local" : "Themyscira",
        "usaCapa" : false,
        "quantidadeGatos" : 2,
        "quantidadeCachorros" : 7
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c3"),
        "nome" : "Capitão América",
        "dateOfBirth" : "1920-07-04T08:30:00.000Z",
        "local" : "América",
        "usaCapa" : false,
        "quantidadeGatos" : 0,
        "quantidadeCachorros" : 9
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c5"),
        "nome" : "Pantera Negra",
        "dateOfBirth" : "1973-11-25T08:30:00.000Z",
        "local" : "Wakanda",
        "usaCapa" : false,
        "quantidadeGatos" : 7,
        "quantidadeCachorros" : 3
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c8"),
        "nome" : "Homem Aranha",
        "dateOfBirth" : "2001-08-10T08:30:00.000Z",
        "local" : "San Francisco",
        "usaCapa" : false,
        "quantidadeGatos" : 0,
        "quantidadeCachorros" : 2
}
```

**9**.Selecione todos os registros em que o nome contenha s.

 ```javascript 
db.Hdeherois.find({ "nome" : /s/ }).pretty()
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c4"),
        "nome" : "Visão",
        "dateOfBirth" : "1940-11-17T08:30:00.000Z",
        "local" : "Nova York",
        "usaCapa" : true,
        "quantidadeGatos" : 4,
        "quantidadeCachorros" : 1
}
```

**10**.Selecione todos os registros em que o nome contenha ‘e’ ou ‘o’.

 ```javascript 
db.Hdeherois.find({ $or:  [{ "nome" : /s/ } , { "nome" : /o/ }]}).pretty()
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750bc"),
        "nome" : "Gavião Arqueiro",
        "dateOfBirth" : "1981-03-18T08:30:00.000Z",
        "local" : "Roma",
        "usaCapa" : false,
        "quantidadeGatos" : 1,
        "quantidadeCachorros" : 0
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750be"),
        "nome" : "Homem Formiga",
        "dateOfBirth" : "1962-01-27T08:30:00.000Z",
        "local" : "Londres",
        "usaCapa" : false,
        "quantidadeGatos" : 4,
        "quantidadeCachorros" : 5
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c1"),
        "nome" : "Deadpool",
        "dateOfBirth" : "1991-04-25T08:30:00.000Z",
        "local" : "Canadá",
        "usaCapa" : false,
        "quantidadeGatos" : 5,
        "quantidadeCachorros" : 3
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c2"),
        "nome" : "Homem de Ferro",
        "dateOfBirth" : "1970-05-29T08:30:00.000Z",
        "local" : "Nova York",
        "usaCapa" : false,
        "quantidadeGatos" : 4,
        "quantidadeCachorros" : 1
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c3"),
        "nome" : "Capitão América",
        "dateOfBirth" : "1920-07-04T08:30:00.000Z",
        "local" : "América",
        "usaCapa" : false,
        "quantidadeGatos" : 0,
        "quantidadeCachorros" : 9
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c4"),
        "nome" : "Visão",
        "dateOfBirth" : "1940-11-17T08:30:00.000Z",
        "local" : "Nova York",
        "usaCapa" : true,
        "quantidadeGatos" : 4,
        "quantidadeCachorros" : 1
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c6"),
        "nome" : "Thor",
        "dateOfBirth" : "1940-05-14T08:30:00.000Z",
        "local" : "Noruega",
        "usaCapa" : true,
        "quantidadeGatos" : 5,
        "quantidadeCachorros" : 3
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c8"),
        "nome" : "Homem Aranha",
        "dateOfBirth" : "2001-08-10T08:30:00.000Z",
        "local" : "San Francisco",
        "usaCapa" : false,
        "quantidadeGatos" : 0,
        "quantidadeCachorros" : 2
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c9"),
        "nome" : "Wolverine",
        "dateOfBirth" : "1880-02-17T08:30:00.000Z",
        "local" : "Canadá",
        "usaCapa" : false,
        "quantidadeGatos" : 3,
        "quantidadeCachorros" : 0
}
```

**11**.Insira 3 novos super-heróis.

 ```javascript 
db.Hdeherois.insertMany([{ 
    "nome" : "Jessica Jones",
    "dateOfBirth" : "2001-02-17T08:30:00.000Z",
    "local" : "NovaYork",
    "usaCapa" : false,
    "quantidadeGatos" : 0,
    "quantidadeCachorros" : 0
},
{
    "nome" : "Tempestade",
    "dateOfBirth" : "1880-02-17T08:30:00.000Z",
    "local" : "Quênia",
    "usaCapa" : true,
    "quantidadeGatos" : 1,
    "quantidadeCachorros" : 0

},
{
    "nome" : "Viúva Negra",
    "dateOfBirth" : "1928-02-17T08:30:00.000Z",
    "local" : "Rússia",
    "usaCapa" : false,
    "quantidadeGatos" : 0,
    "quantidadeCachorros" : 1
}
])
```

**12**.Delete 1 super-herói em que o nome seja igual a Capitão América.

 ```javascript 
db.Hdeherois.remove({_"name": "Capitão America"}) // não é possível fazer pelo name 
//SyntaxError: missing : after property id :

db.Hdeherois.remove({ "_id" : ObjectId("5f99cb2cc645577c0a6750c3") })  
WriteResult({ "nRemoved" : 1 })

//checando se deu certo
db.Hdeherois.find().pretty()
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750bc"),
        "nome" : "Gavião Arqueiro",
        "dateOfBirth" : "1981-03-18T08:30:00.000Z",
        "local" : "Roma",
        "usaCapa" : false,
        "quantidadeGatos" : 1,
        "quantidadeCachorros" : 0
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750bd"),
        "nome" : "Shrek",
        "dateOfBirth" : "1785-04-06T08:30:00.000Z",
        "local" : "Londres",
        "usaCapa" : false,
        "quantidadeGatos" : 5,
        "quantidadeCachorros" : 2
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750be"),
        "nome" : "Homem Formiga",
        "dateOfBirth" : "1962-01-27T08:30:00.000Z",
        "local" : "Londres",
        "usaCapa" : false,
        "quantidadeGatos" : 4,
        "quantidadeCachorros" : 5
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750bf"),
        "nome" : "Batman",
        "dateOfBirth" : "1939-10-01T08:30:00.000Z",
        "local" : "Detroit",
        "usaCapa" : true,
        "quantidadeGatos" : 2,
        "quantidadeCachorros" : 7
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c0"),
        "nome" : "Mulher Maravilha",
        "dateOfBirth" : "1941-12-08T08:30:00.000Z",
        "local" : "Themyscira",
        "usaCapa" : false,
        "quantidadeGatos" : 2,
        "quantidadeCachorros" : 7
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c1"),
        "nome" : "Deadpool",
        "dateOfBirth" : "1991-04-25T08:30:00.000Z",
        "local" : "Canadá",
        "usaCapa" : false,
        "quantidadeGatos" : 5,
        "quantidadeCachorros" : 3
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c2"),
        "nome" : "Homem de Ferro",
        "dateOfBirth" : "1970-05-29T08:30:00.000Z",
        "local" : "Nova York",
        "usaCapa" : false,
        "quantidadeGatos" : 4,
        "quantidadeCachorros" : 1
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c4"),
        "nome" : "Visão",
        "dateOfBirth" : "1940-11-17T08:30:00.000Z",
        "local" : "Nova York",
        "usaCapa" : true,
        "quantidadeGatos" : 4,
        "quantidadeCachorros" : 1
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c5"),
        "nome" : "Pantera Negra",
        "dateOfBirth" : "1973-11-25T08:30:00.000Z",
        "local" : "Wakanda",
        "usaCapa" : false,
        "quantidadeGatos" : 7,
        "quantidadeCachorros" : 3
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c6"),
        "nome" : "Thor",
        "dateOfBirth" : "1940-05-14T08:30:00.000Z",
        "local" : "Noruega",
        "usaCapa" : true,
        "quantidadeGatos" : 5,
        "quantidadeCachorros" : 3
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c7"),
        "nome" : "Hulk",
        "dateOfBirth" : "1969-12-18T08:30:00.000Z",
        "local" : "Novo México",
        "usaCapa" : false,
        "quantidadeGatos" : 1,
        "quantidadeCachorros" : 1
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c8"),
        "nome" : "Homem Aranha",
        "dateOfBirth" : "2001-08-10T08:30:00.000Z",
        "local" : "San Francisco",
        "usaCapa" : false,
        "quantidadeGatos" : 0,
        "quantidadeCachorros" : 2
}
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c9"),
        "nome" : "Wolverine",
        "dateOfBirth" : "1880-02-17T08:30:00.000Z",
        "local" : "Canadá",
        "usaCapa" : false,
        "quantidadeGatos" : 3,
        "quantidadeCachorros" : 0
}
{
        "_id" : ObjectId("5f9a0331a62977dd9e38a93d"),
        "nome" : "Jessica Jones",
        "dateOfBirth" : "2001-02-17T08:30:00.000Z",
        "local" : "NovaYork",
        "usaCapa" : false,
        "quantidadeGatos" : 0,
        "quantidadeCachorros" : 0
}
{
        "_id" : ObjectId("5f9a0331a62977dd9e38a93e"),
        "nome" : "Tempestade",
        "dateOfBirth" : "1880-02-17T08:30:00.000Z",
        "local" : "Quênia",
        "usaCapa" : true,
        "quantidadeGatos" : 1,
        "quantidadeCachorros" : 0
}
{
        "_id" : ObjectId("5f9a0331a62977dd9e38a93f"),
        "nome" : "Viúva Negra",
        "dateOfBirth" : "1928-02-17T08:30:00.000Z",
        "local" : "Rússia",
        "usaCapa" : false,
        "quantidadeGatos" : 0,
        "quantidadeCachorros" : 1
}
```
**13**.Atualize a quantidade de gatos em que o usuário com o registro de nome ‘Thor’ possui. Atualize a quantidade de gatos de ‘5’ para ‘7’.

```javascript
db.Hdeherois.update({ "nome" : "Thor" },{ $set : { "quantidadeGatos" : 7}})
//WriteResult({ "nMatched" : 1, "nUpserted" : 0, "nModified" : 1 })

//checando se deu certo
db.Hdeherois.find({"nome":"Thor"}).pretty()
{
        "_id" : ObjectId("5f99cb2cc645577c0a6750c6"),
        "nome" : "Thor",
        "dateOfBirth" : "1940-05-14T08:30:00.000Z",
        "local" : "Noruega",
        "usaCapa" : true,
        "quantidadeGatos" : 7,
        "quantidadeCachorros" : 3
}
```


**14**.Atualize o registro da Mulher Maravilha para capa = true;

```javascript
db.Hdeherois.update({ "nome" : "Mulher Maravilha" },{ $set : { "usaCapa" : true}})
//WriteResult({ "nMatched" : 1, "nUpserted" : 0, "nModified" : 1 })

//checando se deu certo
db.Hdeherois.find({"nome":"Mulher Maravilha"}).pretty()
{
    "_id" : ObjectId("5f99cb2cc645577c0a6750c0"),
    "nome" : "Mulher Maravilha",
    "dateOfBirth" : "1941-12-08T08:30:00.000Z",
    "local" : "Themyscira",
    "usaCapa" : true,
    "quantidadeGatos" : 2,
    "quantidadeCachorros" : 7
}
```

**15**.colocar o nome em ordem alfabética. (exercício extra que fiz)

```javascript
db.Hdeherois.find({},{nome: 1, _id: 0}).sort({nome: 1}).pretty()
{ "nome" : "Batman" }
{ "nome" : "Deadpool" }
{ "nome" : "Gavião Arqueiro" }
{ "nome" : "Homem Aranha" }
{ "nome" : "Homem Formiga" }
{ "nome" : "Homem de Ferro" }
{ "nome" : "Hulk" }
{ "nome" : "Jessica Jones" }
{ "nome" : "Mulher Maravilha" }
{ "nome" : "Pantera Negra" }
{ "nome" : "Shrek" }
{ "nome" : "Tempestade" }
{ "nome" : "Thor" }
{ "nome" : "Visão" }
{ "nome" : "Viúva Negra" }
{ "nome" : "Wolverine" }
```

**16**.Selecione todos os registros que foram trabalhados e exporte para um arquivo JSON.

```javascript
mongoexport --collection=Hdeherois --db=reprograma --out="C:\Users\naiar\Desktop\DESK\CURSOS\REPROGRAMA\semana12\arquivo-json\herois.json"

{"_id":{"$oid":"5f99cb2cc645577c0a6750bc"},"nome":"Gavião Arqueiro","dateOfBirth":"1981-03-18T08:30:00.000Z","local":"Roma","usaCapa":false,"quantidadeGatos":1,"quantidadeCachorros":0}
{"_id":{"$oid":"5f99cb2cc645577c0a6750bd"},"nome":"Shrek","dateOfBirth":"1785-04-06T08:30:00.000Z","local":"Londres","usaCapa":false,"quantidadeGatos":5,"quantidadeCachorros":2}
{"_id":{"$oid":"5f99cb2cc645577c0a6750be"},"nome":"Homem Formiga","dateOfBirth":"1962-01-27T08:30:00.000Z","local":"Londres","usaCapa":false,"quantidadeGatos":4,"quantidadeCachorros":5}
{"_id":{"$oid":"5f99cb2cc645577c0a6750bf"},"nome":"Batman","dateOfBirth":"1939-10-01T08:30:00.000Z","local":"Detroit","usaCapa":true,"quantidadeGatos":2,"quantidadeCachorros":7}
{"_id":{"$oid":"5f99cb2cc645577c0a6750c0"},"nome":"Mulher Maravilha","dateOfBirth":"1941-12-08T08:30:00.000Z","local":"Themyscira","usaCapa":true,"quantidadeGatos":2,"quantidadeCachorros":7}
{"_id":{"$oid":"5f99cb2cc645577c0a6750c1"},"nome":"Deadpool","dateOfBirth":"1991-04-25T08:30:00.000Z","local":"Canadá","usaCapa":false,"quantidadeGatos":5,"quantidadeCachorros":3}
{"_id":{"$oid":"5f99cb2cc645577c0a6750c2"},"nome":"Homem de Ferro","dateOfBirth":"1970-05-29T08:30:00.000Z","local":"Nova York","usaCapa":false,"quantidadeGatos":4,"quantidadeCachorros":1}
{"_id":{"$oid":"5f99cb2cc645577c0a6750c4"},"nome":"Visão","dateOfBirth":"1940-11-17T08:30:00.000Z","local":"Nova York","usaCapa":true,"quantidadeGatos":4,"quantidadeCachorros":1}
{"_id":{"$oid":"5f99cb2cc645577c0a6750c5"},"nome":"Pantera Negra","dateOfBirth":"1973-11-25T08:30:00.000Z","local":"Wakanda","usaCapa":false,"quantidadeGatos":7,"quantidadeCachorros":3}
{"_id":{"$oid":"5f99cb2cc645577c0a6750c6"},"nome":"Thor","dateOfBirth":"1940-05-14T08:30:00.000Z","local":"Noruega","usaCapa":true,"quantidadeGatos":7.0,"quantidadeCachorros":3}
{"_id":{"$oid":"5f99cb2cc645577c0a6750c7"},"nome":"Hulk","dateOfBirth":"1969-12-18T08:30:00.000Z","local":"Novo México","usaCapa":false,"quantidadeGatos":1,"quantidadeCachorros":1}
{"_id":{"$oid":"5f99cb2cc645577c0a6750c8"},"nome":"Homem Aranha","dateOfBirth":"2001-08-10T08:30:00.000Z","local":"San Francisco","usaCapa":false,"quantidadeGatos":0,"quantidadeCachorros":2}
{"_id":{"$oid":"5f99cb2cc645577c0a6750c9"},"nome":"Wolverine","dateOfBirth":"1880-02-17T08:30:00.000Z","local":"Canadá","usaCapa":false,"quantidadeGatos":3,"quantidadeCachorros":0}
{"_id":{"$oid":"5f9a0331a62977dd9e38a93d"},"nome":"Jessica Jones","dateOfBirth":"2001-02-17T08:30:00.000Z","local":"NovaYork","usaCapa":false,"quantidadeGatos":0.0,"quantidadeCachorros":0.0}
{"_id":{"$oid":"5f9a0331a62977dd9e38a93e"},"nome":"Tempestade","dateOfBirth":"1880-02-17T08:30:00.000Z","local":"Quênia","usaCapa":true,"quantidadeGatos":1.0,"quantidadeCachorros":0.0}
{"_id":{"$oid":"5f9a0331a62977dd9e38a93f"},"nome":"Viúva Negra","dateOfBirth":"1928-02-17T08:30:00.000Z","local":"Rússia","usaCapa":false,"quantidadeGatos":0.0,"quantidadeCachorros":1.0}

```


