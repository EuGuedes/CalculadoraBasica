# CalculadoraBasica
Repositório de estudo <!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculadora Simples</title>
    <style>
        *{
            margin: 0;
            padding: 0;
        }
        .fundo{
            background-image:linear-gradient(45deg,rgb(0, 0, 0), rgb(185, 16, 53));
            height: 100vh;
            color:#fff;
            font-family: Arial, Helvetica, sans-serif;
            text-align: center;
        }
        .calculadora{
            position: absolute;
            background-color:rgba(68, 11, 38, 0.884);
            top: 10%;
            left: 40%;
            right: 40%;
            font-weight: 200px;
            transform: translate(5%,25%);
            border-radius: 20px;
            padding: 40px;
        }
        .botao{
            width: 50px;
            height: 50px;
            font-size: 25px;
            cursor: pointer;
            margin: 3px;
            background-color: rgb(0, 0, 0); 
            border: none;
            color: #fff;
        }
        .botao:hover{
            background-color: black;
        }
         #resultado{
            background-color: whitesmoke;   
            width: 218px;
            height: 30px;
            margin: 5px;
            font-size: 25px;
            color: black;
            text-align: right;
            padding: 1px;
           
         }
    </style>
</head>
<body>
    <div class="fundo">
      <h1>João Guedes</h1>
     <div class= "calculadora">
         <h1>Calculadora</h1>
    <p id="resultado"></p>
    <table> 
        <tr>
            <td> <button class="botao" onclick="clean()">C</button></td>
            <td> <button class="botao" onclick="back()"><</button></td>
            <td> <button class="botao" onclick="insert('/')">/</button></td>
            <td> <button class="botao" onclick="insert('*')">x</button></td>
        </tr>
       
        <tr>
            <td> <button class="botao" onclick="insert('7')">7</button></td>
            <td> <button class="botao" onclick="insert('8')">8</button></td>
            <td> <button class="botao" onclick="insert('9')">9</button></td>
            <td> <button class="botao" onclick="insert('-')">-</button></td>
        </tr>
       
        <tr>
            <td> <button class="botao" onclick="insert('4')">4</button></td>
            <td> <button class="botao" onclick="insert('5')">5</button></td>
            <td> <button class="botao" onclick="insert('6')">6</button></td>
            <td> <button class="botao" onclick="insert('+')">+</button></td>
        </tr>

        <tr>
            <td> <button class="botao" onclick="insert('1')">1</button></td>
            <td> <button class="botao" onclick="insert('2')">2</button></td>
            <td> <button class="botao" onclick="insert('3')">3</button></td>
            <td colspan="2"> <button class="botao" style="height: 50px;" onclick="calcular()">=</button></td>
        </tr>
        <tr>
            <td colspan="2"> <button class="botao" style="width: 105px;"  onclick="insert('0')">0</button></td>
            <td colspan="2"> <button class="botao" style="width: 105px;" onclick="insert('.')">.</button></td>
        </tr>
    </table>
     </div>
    </div>
    <script>
function insert(num)
{
var numero = document.getElementById('resultado').innerHTML;
document.getElementById('resultado').innerHTML = numero + num;
}
function clean()
{
    document.getElementById('resultado').innerHTML = "";
}
function back() 
{
    var resultado = document.getElementById('resultado').innerHTML;
    document.getElementById('resultado').innerHTML = resultado.substring(0, resultado.length -1);
}
function calcular()
{
    var resultado = document.getElementById('resultado').innerHTML;
    if (resultado)
    {
        document.getElementById('resultado').innerHTML = eval(resultado)
    }
    else
    {
        document.getElementById('resultado').innerHTML = 'Nada...FDP?'

    }
}
    </script>


</body>
</html>


<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculadora Simples</title>
    <style>
        *{
            margin: 0;
            padding: 0;
        }
        .fundo{
            background-image:linear-gradient(45deg,rgb(0, 0, 0), rgb(185, 16, 53));
            height: 100vh;
            color:#fff;
            font-family: Arial, Helvetica, sans-serif;
            text-align: center;
        }
        .calculadora{
            position: absolute;
            background-color:rgba(68, 11, 38, 0.884);
            top: 10%;
            left: 40%;
            right: 40%;
            font-weight: 200px;
            transform: translate(5%,25%);
            border-radius: 20px;
            padding: 40px;
        }
        .botao{
            width: 50px;
            height: 50px;
            font-size: 25px;
            cursor: pointer;
            margin: 3px;
            background-color: rgb(0, 0, 0); 
            border: none;
            color: #fff;
        }
        .botao:hover{
            background-color: black;
        }
         #resultado{
            background-color: whitesmoke;   
            width: 218px;
            height: 30px;
            margin: 5px;
            font-size: 25px;
            color: black;
            text-align: right;
            padding: 1px;
           
         }
    </style>
</head>
<body>
    <div class="fundo">
      <h1>João Guedes</h1>
     <div class= "calculadora">
         <h1>Calculadora</h1>
    <p id="resultado"></p>
    <table> 
        <tr>
            <td> <button class="botao" onclick="clean()">C</button></td>
            <td> <button class="botao" onclick="back()"><</button></td>
            <td> <button class="botao" onclick="insert('/')">/</button></td>
            <td> <button class="botao" onclick="insert('*')">x</button></td>
        </tr>
       
        <tr>
            <td> <button class="botao" onclick="insert('7')">7</button></td>
            <td> <button class="botao" onclick="insert('8')">8</button></td>
            <td> <button class="botao" onclick="insert('9')">9</button></td>
            <td> <button class="botao" onclick="insert('-')">-</button></td>
        </tr>
       
        <tr>
            <td> <button class="botao" onclick="insert('4')">4</button></td>
            <td> <button class="botao" onclick="insert('5')">5</button></td>
            <td> <button class="botao" onclick="insert('6')">6</button></td>
            <td> <button class="botao" onclick="insert('+')">+</button></td>
        </tr>

        <tr>
            <td> <button class="botao" onclick="insert('1')">1</button></td>
            <td> <button class="botao" onclick="insert('2')">2</button></td>
            <td> <button class="botao" onclick="insert('3')">3</button></td>
            <td colspan="2"> <button class="botao" style="height: 50px;" onclick="calcular()">=</button></td>
        </tr>
        <tr>
            <td colspan="2"> <button class="botao" style="width: 105px;"  onclick="insert('0')">0</button></td>
            <td colspan="2"> <button class="botao" style="width: 105px;" onclick="insert('.')">.</button></td>
        </tr>
    </table>
     </div>
    </div>
    <script>
function insert(num)
{
var numero = document.getElementById('resultado').innerHTML;
document.getElementById('resultado').innerHTML = numero + num;
}
function clean()
{
    document.getElementById('resultado').innerHTML = "";
}
function back() 
{
    var resultado = document.getElementById('resultado').innerHTML;
    document.getElementById('resultado').innerHTML = resultado.substring(0, resultado.length -1);
}
function calcular()
{
    var resultado = document.getElementById('resultado').innerHTML;
    if (resultado)
    {
        document.getElementById('resultado').innerHTML = eval(resultado)
    }
    else
    {
        document.getElementById('resultado').innerHTML = 'Nada...FDP?'

    }
}
    </script>


</body>
</html>
