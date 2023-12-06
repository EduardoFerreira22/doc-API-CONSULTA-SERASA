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











