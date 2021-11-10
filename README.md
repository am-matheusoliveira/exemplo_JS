# primeiro_exemplo
Nesse ficara pequenos exemplos de códigos para estudos e trabalhos. 

#Abaixo temos um pouco de JAvaScript

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML & JS</title>
    <script>

        var diaSemana = prompt("Dia da Semana:", "Digite o Dia da Semana!");
        var dias = new Array();        
        dias = (["Domingo", "Segunda-Feira", "Terça-Feira", "Quarta-Feira", "Quinta-Feira", "Sexta-Feira", "Sabado"]);    

        if(diaSemana != null){
            for(var cont = 0; cont <= dias.length; cont++){
                if(cont != dias.length){
                    var certeza = window.confirm(dias[cont]);
                    if(certeza){
                        var frutas = new Array("Maçã", "Pera", "Uva", "Morango");
                        var resposta = window.prompt("Qual fruta você mais come?","Digite sua resposta!");
                        var resultado = frutas.indexOf(resposta);
                        if(resultado != -1){
                            alert("Meus parabens você escolheu uma das 4 frutas premiadas! Fruta: "+frutas[resultado]);
                            //!= Nesse momento a expressão abaixo e != de undefined
                            //Vamos mudar para 'defined'
                            var obj = frutas[resultado];
                            if (typeof obj !== 'undefined') {
                                // your code here
                                alert("Objeto exitente: "+frutas[resultado]);
                            }
                       }
                    }
                }                
            }
        };
    </script>
</head>
<body>
    
</body>
</html>
