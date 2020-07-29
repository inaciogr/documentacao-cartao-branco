# Qual objetivo do método PUT do REST \ HTTP?

O método PUT é utilizado para atualização completa de um determinado recurso, como por exemplo?

```
PUT http://localhost:80808/v1/carros/cc0cfe13-edce-4fe4-a12d-90b32bb844ba

{
   "nome" : "Gol",
   "ano" : 2019
}
```

Olhando o método e o recurso sabemos que estamos atualizando todos os atributos do carro com o identificador 
`cc0cfe13-edce-4fe4-a12d-90b32bb844ba`.

De acordo com a especificação do REST, caso o recurso não for encontrado deve-se gerar um, ou seja, caso o carro com o
identificador `cc0cfe13-edce-4fe4-a12d-90b32bb844ba` não existir, devemos criar um novo.

Porém essa pratica não é muito aplicada pelo mercado, pois utiliza-se o método POST para tal objetivo.