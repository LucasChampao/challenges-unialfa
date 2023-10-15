## Itens Feitos:

* Exercícios Feitos 16 ao 21, como solicitado em sala de aula;

### Exercício 18 [PHP BÁSICO];

* Construir um algoritmo que leia 2 números e efetue a adição. Caso o valor somado seja maior que 20, deverá ser apresentado somando-se a ele mais 8; caso o valor somado seja menor ou igual a 20, este deverá ser apresentado subtraindo-se 5.


~~~ PHP

<?php

echo "<h2> Exercicio 18 </h2>"; // - 18

$num1 = 12;
$num2 = 5;
$resul = $num1 + $num2;

echo "Número 1 é : $num1 <br>";
echo "Número 2 é : $num2 <br>";

echo "<h6> Resultado: $resul </h6>";

if ($resul > 20) {
    $resul += 8;
    echo $resul;
} else if ($resul <= 20) {
    $resul -= 5;
    echo $resul;
}
?>

~~~

