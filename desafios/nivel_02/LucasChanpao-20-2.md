## Itens Feitos:

* Exercícios Feitos 16 ao 21, como solicitado em sala de aula;

### Exercício 20 [PHP BÁSICO];

* A biblioteca de uma universidade deseja fazer um algoritmo que leia o nome do livro que será emprestado,
 o tipo de usuário (professor ou aluno)
 e possa imprimir um recibo conforme mostrado a seguir. Considerar que o 
 professor tem 10 dias para devolver o livro o aluno somente 3 dias.

~~~ html
<div class="container">
    <form action="ex20.php" method="POST">
        <div class="row">
            <div class="col-6">
                <label for="exampleFormControlInput1" class="form-label"> <strong> Digite o Nome do Livro: </strong>
                </label>
                <input type="text" class="form-control" id="exampleFormControlInput1" name="livro" placeholder=" Os 3 porquinhos... ">
                <label for="exampleFormControlInput1" class="form-label"> <strong> Digite o seu nome: </strong>
                </label>
                <input type="text" class="form-control" id="exampleFormControlInput1" name="nome" placeholder=" Alex Morgado... ">
                <label for="exampleFormControlInput1" class="form-label"> <strong> Digite o seu Curso: </strong>
                </label>
                <input type="text" class="form-control" id="exampleFormControlInput1" name="Curso" placeholder=" Sistemas...">
                <label for="exampleFormControlInput1" class="form-label"> <strong> Você é: </strong></label><br>

                <div class="form-check">
                    <input class="form-check-input" type="checkbox" name="Aluno" id="flexCheckDefault">
                    <label class="form-check-label" for="flexCheckDefault">
                        Aluno
                    </label>
                </div>
                <div class="form-check">
                    <input class="form-check-input" type="checkbox" name="Professor" id="flexCheckChecked">
                    <label class="form-check-label" for="flexCheckChecked">
                        Professor
                    </label>
                </div>
                <button type="submit" class="btn btn-success">Enviar</button>

            </div>
        </div>
    </form>
</div>
~~~

--- ex20.php ---

~~~ Php
<?php

echo "NOME DO LIVRO: <br>" . $_POST['livro'] . "<br>";
echo "NOME DO ALUNO: <br>" . $_POST['nome'] . "<br>";
echo "CURSO: " . $_POST['Curso'] . "<br>";


if (isset($_POST['Aluno'])) {
    echo "=== ALUNO=== DEVOLVER EM 3 DIAS, EM CASO DE ATRASO COBRAR MULTA POR DIA DE ATRASO  !!";
} else {
    echo  "=== PROFESSOR === DEVOLVER EM 10 DIAS, EM CASO DE ATRASO COBRAR MULTA POR DIA DE ATRASO  !!";
}
<?
~~~
