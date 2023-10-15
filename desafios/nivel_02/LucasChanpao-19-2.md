## Itens Feitos:

* Exercícios Feitos 16 ao 21, como solicitado em sala de aula;

### Exercício 19 [PHP BÁSICO];

* Ler um número inteiro entre 1 e 12 e escrever o mês correspondente.
 Caso o número seja fora desse intervalo, 
 informar que não existe mês com este número.

~~~ HTML 

<div class="container">
    <form action="ex19.php" method="POST">
        <div class="row">
            <div class="col-6">
                <label for="exampleFormControlInput1" class="form-label"> <strong> Digite um número Inteiro entre 1 e
                        12: </strong> </label>
                <input type="text" class="form-control" id="exampleFormControlInput1" name="Numeroint" placeholder=" 1, 2, 3, 4, 5, 6, 7...">
                <button type="submit" class="btn btn-success">Enviar</button>
            </div>
        </div>
    </form>
</div>
~~~

--- ex19.php --- 

~~~ Php
<?php
var_dump($_POST);
echo '<br>';

$mes = $_POST['Numeroint'];

switch ($mes) {
  case 1:
    echo "<h2>MÊS JANEIRO </h2>";
    break;
  case 2:
    echo "<h2>MÊS FEVEREIRO </h2>";
    break;
  case 3:
    echo "<h2>MÊS MARÇO</h2>";
    break;
  case 4:
    echo "<h2>MÊS ABRIL</h2>";
    break;
  case 5:
    echo "<h2>MÊS MAIO </h2>";
    break;
  case 6:
    echo "<h2>MÊS JUNHO</h2>";
    break;
  case 7:
    echo "<h2>MÊS JULHO</h2>";
    break;
  case 8:
    echo "<h2>MÊS AGOSTO</h2>";
    break;
  case 9:
    echo "<h2>MÊS SETEMBRO</h2>";
    break;
  case 10:
    echo "<h2>MÊS OUTUBRO</h2>";
    break;
  case 11:
    echo "<h2>MÊS NOVEMBRO</h2>";
    break;
  case 12:
    echo "<h2>MÊS DEZEMBRO</h2>";
    break;
  default:
    echo "<h2>Não existe mês com este número.</h2>";
};
?>
~~~



