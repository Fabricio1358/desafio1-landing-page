# desafio1-landing-page

Desafio 1 - Landing Page do Curso de Tecnologia da Escola DNC

###Links:

https://dnc-desafio-1-landing-page.netlify.app
https://docs.google.com/spreadsheets/d/1of7rzuRTyqO-oJ0yHFqQoxeKcP_OIcuWABkZBKKkvtE/edit#gid=0

#HTML

##Estrutura

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600;700;800;900&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="style.css">
    <title> Desafio 1: Landing Page </title>
</head>
<body>
    <!-- Seção Margem -->
    <div id="margem"> <h1 id="titulo-margem"> Tradição em projetos de arquitetura </h1>
        <p id="descricao-margem"> Arquitetura residencial e comercial. </p>
    </div>
    <!-- Seção Características -->
    <div id="caracteristicas">
        <div> <h2 class="valor-caracteristicas"> 850 </h2> <p class="descricao-caracteristicas"> empreendimentos construídos </p> </div> 
        <div> <h2 class="valor-caracteristicas"> 40 </h2> <p class="descricao-caracteristicas"> anos de mercado e experiência </p> </div> 
        <div> <h2 class="valor-caracteristicas"> 2,000,000 </h2> <p class="descricao-caracteristicas">  m² em projetos construídos </p> </div>         
    </div>
    <!-- Seção Imagem -->
    <div id="imagem"> 
        <img id="img-obra" src="Imagens/img-obra.svg" alt="ERRO">
        <h1 id="titulo-imagem" class="descricao-imagem"> Arquitetos com História e Experiência. </h1> 
        <p id="texto-imagem" class="descricao-imagem"> Nós realizamos desde 2002 projetos e gerenciamento de obras. <br>
            Com mais de 800 projetos e 2.000.000 de m² construídos, tendo <br>
            como principal proposta transformar em realidade os sonhos de <br>
            seus clientes, criando projetos personalizados, unindo a tradição <br>
            e a modernidade em nossos projetos.
        </p>
    </div>
    <!-- Seção Formulário -->
    <div id="formulario"> 
        <h1 id="titulo-formulario"> Conheça mais sobre nossos serviços: </h1> <br> <br> <br>
        <form action="https://api.sheetmonkey.io/form/nTLmL1ttCn9cwLXhsTxBmH" method="POST">
            <input class="caixas" id="nome" type="text" placeholder="Nome" name="Name" required> <br> <br> <br>
            <input class="caixas" id="email" type="email" placeholder="Email" name="Email" required> <br> <br> <br>
            <input type="hidden" name="Created" value="x-sheetmonkey-current-date-time" />
            <button type="submit"> Fale Conosco </button> 
        </form> 
    </div>   
    <script src="index.js"></script>
</body>
</html>

#CSS

##Estrutura

*{
    margin: 0px;
    font-family: 'inter';
}
/* Estilo da Margem */
#margem{
    background-color: #303030;
    padding: 100px;
    color: #FFFFFF;
    padding-left: 50px;
}

#titulo-margem{
    font-size: 55px;
    margin-top: 80px;
}

#descricao-margem{
    margin-top: 30px;
    padding-bottom: 50px;
    font-size: 20px;
}
/* Estilo das Características*/
#caracteristicas{
    background-color: #F9F9F9;
    display: grid;
    grid-auto-flow: column;
    padding-top: 80px;
    padding-left: 10%;
    padding-bottom: 80px;
    text-align: center
}

.valor-caracteristicas{
    font-size: 40px;
    text-align: left;
}
   
.descricao-caracteristicas{
    font-size: 20px;
    text-align: left;
}
/* Estilo da Seção Imagem*/
#imagem{
    margin-bottom: 250px;
    margin-top: 50px;
}

#img-obra{
    float: right;
    margin-right: 4%;
    width: 450px;
    height: 550px;
}

.descricao-imagem{
    margin-left: 5%;
    padding-top: 13%;
}

#titulo-imagem{
    font-size: 35px;
    margin-bottom: 70px;
    margin-right: 20px;
}

#texto-imagem{
    font-size: 20px;
    padding-top: 0px;
}
/* Estilo do Formulário*/
#formulario{
    background-color: #303030;
    padding-bottom: 60px;
    text-align: center;
}

#titulo-formulario{
    font-size: 32px;
    color: #FFFFFF;
    text-align: center;
    padding-top: 80px;
}

input{
    width: 450px;
    height: 60px;
    padding-left: 15px;
    border: 0px;
    border-radius: 10px;
    font-size: 18px;
}

button{
    width: 250px;
    height: 60px;
    background-color: #C07212;
    border: 0px;
    border-radius: 10px;
    font-size: 25px;
    color: #FFFFFF;
    cursor: pointer;
}

button:hover{
    background-color: #d8a363;
    color: white;
    box-shadow: 0px 10px 10px rgb(32, 32, 32);
    transform: translateY(-10px);
    transition-duration: 0.3s;
} 
