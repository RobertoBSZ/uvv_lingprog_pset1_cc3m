# Validador de cartão
## PSET-01
Este trabalho foi criado pelo aluno Roberto Bastos Souza, do curso de Ciência da Computação e turma CC3M da Universidade Vila Velha
Professor: Abrantes

## Função "input_cartao()"
A função "input_cartao" é responsável por pegar o número do cartão que o usuário digitar, remover tudo que não for um número da string, colocar em uma lista todos os caracteres da string e, por fim, transformar a lista de string em uma lista de inteiros e retornar esta lista, para que seja possível realizar operações matemáticas na função "valida_cartao".

## Função "valida_cartao(nmr)"
A função "valida_cartao" é responsável por validar o número do cartão que o usuário digitou na função "input_cartao". Primeiro passo é contar e pegar os números de trás pra frente, de dois em dois, a partir do penúltimo item da lista e multiplicar por dois. Caso o resultado da multiplicação de alguns números seja maior que 9, é feita uma subtração por 9, que é como se fosse a soma dos algoritmos daquele número. 'Ex= 12: 1 + 2 = 3 | 12 - 9 = 3'. Após a multiplicação dos números, eles são adicionados em uma nova lista, a lista_numrcard_final, e é feito uma nova contagem na lista anterior para pegar os números que não foram selecionados e adiciona-los nessa nova lista. Por fim, é feito uma soma nessa nova lista 'lista_numrcard_final' e, caso o resto da divisão dessa soma por 10 seja 0, o código irá printar a bandeira do cartão. Caso o resto não seja 0, o código irá printar "inválido". Além disso, caso o código não tenha no mínimo 13 dígitos (Visa) ou no máximo 16 dígitos (Visa e MasterCard), o código também printará "inválido".

## Informações adicionais
Este código é o Algoritmo de Luhn, que verifica se o número do cartão é válido sintaticamente. Ele identifica apenas as bandeiras AMEX, VISA ou MASTERCARD.
