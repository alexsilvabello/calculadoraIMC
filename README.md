
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calcula IMC</title>
</head>
<body>
        <script>

                function pulaLinha() {

                    document.write("<br>");
                    document.write("<br>");
            }

                function mostra(frase) {

                    document.write(frase);
                    pulaLinha();
            }

                function calculaImc(altura, peso) {

                    return peso / (altura * altura);
            }

            var nome = prompt("Digite seu nome");
            var alturaInformada = prompt(nome + " Informe sua altura");
            var pesoInformado = prompt(nome + " Informe seu peso");
            var imc = calculaImc(alturaInformada, pesoInformado)

            document.write(nome + ", o seu IMC é " + Math.round(imc));

            if(imc < 18.5) {

            mostra(" Você está abaixo do recomendado");

            }

            if(imc > 35) {

            mostra(" Você está acima do recomendado");
            }

            if(imc >= 18.5 && imc <= 35) {

            mostra(" Seu IMC está excelente!");

            }

            
        </script>
</body>
</html>
