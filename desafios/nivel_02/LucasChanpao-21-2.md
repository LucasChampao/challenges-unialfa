## Itens Feitos:

* Exercícios Feitos 16 ao 21, como solicitado em sala de aula;

### Exercício 21 [PHP BÁSICO];

* Crie um lista de contas correntes, contendo 4 contas bancárias. 
Em cada conta deve ter os seguintes dados: titular e saldo.
Imprima em um echo os nomes dos titulares.


~~~ php
<?php
$contasbancarias = [
    ["titular" => "Lucas Rodrigues", "saldo" => 2000],
    ["titular" => "Alex Morgado", "saldo" => 50000],
    ["titular" => "Matheus Urbano", "saldo" => 1200],
    ["titular" => "Leticia Pereira", "saldo" => 250]
];

foreach ($contasbancarias as $correntes) {
    echo "Nome Titular: " . $correntes["titular"] . "<br>";
    //echo "Saldo: ". $correntes["saldo"]."<br>";
};
?>
~~~ 


