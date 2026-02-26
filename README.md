# Atividade de PHP - Array com a palavra "UNIASSELVI"

## 📌 Descrição
Este repositório contém a resolução de uma atividade da disciplina de Linguagens de Programação, do 3º semestre do curso de Análise e Desenvolvimento de Sistemas. O objetivo era criar um script em PHP que manipulasse arrays para exibir cada letra da palavra "UNIASSELVI" com seu respectivo índice.

## 🧩 Enunciado
Crie uma página PHP que declare um array, onde cada elemento corresponda a uma letra da palavra **"UNIASSELVI"**. Em seguida, imprima o valor do array, separado por linhas e indicando o índice da posição que está sendo impressa.

A saída esperada é:
# php-array-string-uniasselevi
    Script PHP que transforma a string "UNIASSELVI" em um array e exibe cada letra com seu respectivo índice. Exercício da disciplina Linguagens de Programação - 3° semestre ADS.
0: U
1: N
2: I
3: A
4: S
5: S
6: E
7: L
8: V
9: I

## 💡 Solução proposta
Foi utilizada a função `str_split()` para transformar a string em um array de caracteres, e um loop `foreach` para percorrer o array e exibir cada elemento com seu índice.

### Código PHP
```php
<?php
$palavra = "UNIASSELVI";
$letras = str_split($palavra); // Converte a string em array

foreach ($letras as $indice => $letra) {
    echo $indice . ": " . $letra . "<br>";
}
?>
Explicação do código

    str_split('UNIASSELVI') : divide a string em um array, onde cada posição contém uma letra.

    foreach ($letras as $indice => $letra) : percorre o array, capturando o índice numérico (0, 1, 2...) e o valor (a letra correspondente).

    echo $indice . ": " . $letra . "<br>" : imprime o índice e a letra, com uma quebra de linha HTML para exibição no navegador.
