# API CONSULTA SERASA 📜

Essa API fornece a possibilidade de fazer consultas diretamente no Serasa.

## URL BASE

 `https://api-serasa.sollosconsultas.com.br`

## Rotas 


 `post` **/login**

body:
```
{
	"user_login":"gstv",
	"password_login":"Gustavo123"
}
```

<br>
<br>
<br>





 `get` **/top-score/pf/:documentNumber**

Exemplo: /top-score/pf/00000001163

Headers:
```
{
	"x-access-token":"token recebido pela rota /login",
}
```

<br>
<br>
<br>





 `get` **/top-score/pj/:documentNumber**

Exemplo: /top-score/pj/00000028000129

Headers:
```
{
	"x-access-token":"token recebido pela rota /login",
}
```

<br>
<br>
<br>





 `get` **/combo-concessao/:documentNumber**

Exemplo: /combo-concessao/00000001163

Headers:
```
{
	"x-access-token":"token recebido pela rota /login",
}
```

<br>
<br>
<br>





 `get` **/consultas**

Verifica o numero de consultas feitas e o saldo em centavos disponivel

Headers:
```
{
	"x-access-token":"token recebido pela rota /login",
}
```

<br>
<br>
<br>




## ROTAS PARA ADMIN

 `post` **/add-saldo**

Verifica o numero de consultas feitas e o saldo disponivel

o valor do saldo deve ser informado em centavos

Headers:
```
{
	"x-access-token":"token recebido pela rota /login",
}
```

<br>

Body:
```
{
	"user": "gstv",
	"saldo":10000
}
```

<br>
<br>
<br>





 `post` **/add-user**

Adiciona um usuario

o "role" pode ser tanto admin ou cliente

Headers:
```
{
	"x-access-token":"token recebido pela rota /login",
}
```

<br>

Body:
```
{
	"name":"gustavo",
	"user": "gstv",
	"password": "Gustavo123",
	"role":"admin"
}
```

<br>
<br>
<br>





 `get` **/list-user**

Lista todas informações de todos os usuario

Headers:
```
{
	"x-access-token":"token recebido pela rota /login",
}
```

<br>
<br>
<br>





 `delete` **/delete-user/:user**

Exemplo: /delete-user/gstv

Deleta um usuario

Headers:
```
{
	"x-access-token":"token recebido pela rota /login",
}
```

<br>
<br>
<br>







