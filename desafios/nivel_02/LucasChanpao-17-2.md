## Itens Feitos:

* Exercícios Feitos 16 ao 21, como solicitado em sala de aula;

### Exercício 17 [PHP BÁSICO];

* Cálculo Imc;

-----------------------------------------------------------------------------------------------------------------------

~~~ PHP

<?php
echo "<h2> EXERCÍCIO 17 </h2>"; // - 17
?>
~~~

~~~ HTML
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CHALLENGE PHP</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-9ndCyUaIbzAi2FUVXJi0CjmCapSmO7SnpJef0486qhLnuZ2cdeRhO02iuK6FUUVM" crossorigin="anonymous">
</head>

<body>
    <div class="container">
        <form action="dados.php" method="POST">
            <div class="row">
                <div class="col-6">
                    <label for="exampleFormControlInput1" class="form-label">Altura: </label>
                    <input type="text" class="form-control" id="exampleFormControlInput1" name="Altura" placeholder="Digite Sua Altura">
                </div>
                <div class="col-6">
                    <label for="exampleFormControlInput1" class="form-label">Peso: </label>
                    <input type="text" class="form-control" id="exampleFormControlInput1" name="Peso" placeholder="Digite Seu peso">
                    <button type="submit" class="btn btn-success">Enviar</button>

                </div>
            </div>
        </form>
    </div>
</body>
</html>
~~~

~~~ PHP
--- dados.php ---
<?php

var_dump($_POST);
echo "<br>";

$peso = $_POST['Peso'];
$altura = $_POST['Altura'];

echo "Peso: " . $peso . "<br>";
echo "Altura: " . $altura . "<br>";

$imc = $peso /= ($altura * 2);
$imc = round($imc * 100, 2);

echo " Seu IMC é: " . $imc . "<br>";

if ($imc <= 18.5) {
    echo " <h2>Abaixo do peso</h2>";
} else if ($imc >= 18.6 && $imc < 24.9) {
    echo "<h2>Peso Ideal <Parabens></h2>";
} else if ($imc >= 25.0 && $imc < 29.9) {
    echo "<h2>Levemente acima do peso !!</h2> ";
} else if ($imc >= 30.0 && $imc < 34.9) {
    echo "<h2>Obsidade Grau 1</h2>";
} else if ($imc >= 35.0 && $imc < 39.9) {
    echo "<h2>Obsidade Grau 2</h2>";
} else {
    echo "<h2>Obsidade Grau 3 < Mórbida ></h2>";
}
/* EXERCÍCIO 17 */
?>
~~~



