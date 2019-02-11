# Loja StarWars

O desafio consiste em criar uma loja de itens de Star Wars que o usuário é capaz de adicionar os itens desejados em um carrinho de compras e finalizar a compra com uma simulação de transação e-commerce.

O candidato deve dar **fork** neste repositório e após o termino do desenvolvimento, realizar um **pull request** para análise do time.

O código deve ser feito na ferramenta Android Studio. Pode ser em Java ou em Kotlin.

###### Lista de itens

Para obter os itens da loja, sua aplicação deverá realizar uma chamada `GET` na URL https://raw.githubusercontent.com/Felcks/desafio-mobile-lemobs/master/products.json

A lista de itens deve exibir as seguintes informações:
+ Nome [title]
+ Preço [price]
+ Vendedor [seller]
+ Foto do item [thumbnailHd]

Após adicionado ao carrinho, o item não pode ser adicionado de novo. O aplicativo deve deixar isso bem claro: "Produto já adicionado ao carrinho".

###### Carrinho de Compras

O aplicativo deve mostrar um carrinho de compras com os itens adicionados e suas respectivas quantidades.
É possível aumentar a quantidade de itens.

###### Simulação de confirmação de Compra

Para finalizar a compra o usuário deve inserir os seguintes dados fictícios:
+ Número do cartão (com exatos 16 números - XXXX XXXX XXXX XXXX)
+ Nome do portador do cartão
+ Vencimento do cartão (MM/yy) - A data deve ser maior que a atual.
+ CVV (código encontrado na parte traseira do cartão)
+ Valor da transação (total dos itens no carrinho)

Se todos os dados estiverem de acordo, o aplicativo confirma a compra e volta para a tela inicial.

###### Banco de dados
Todas as transações realizadas devem ser salvas em um banco interno com os seguintes campos:
+ Valor
+ Data e hora
+ Últimos 4 dígitos do cartão
+ Nome do portador do cartão

###### Resumo do Aplicativo
+ Tela Lista de Itens
+ Tela Carrinho de Compras
+ Tela Transações Feitas
+ Tela Confirmação de Compra

###### Bônus
+ Conseguir dar Zoom nos produtos
+ Criatividade na organização das telas do aplicativo
+ Salvar, além da transação, os itens que foram comprados
