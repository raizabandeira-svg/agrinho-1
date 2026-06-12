<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Raízes Verdes - Futuro Sustentável</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, sans-serif;
}

body{
    background:#cfeeff;
}

#login{
    min-height:100vh;
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    text-align:center;
    padding:20px;
}

#login h1{
    font-size:60px;
    color:#0c7a2f;
}

#login h2{
    color:#0d47a1;
    margin-bottom:40px;
}

#login input{
    width:350px;
    padding:15px;
    border:none;
    border-radius:10px;
    font-size:18px;
    margin-bottom:20px;
}

#login button{
    background:#0d6efd;
    color:white;
    border:none;
    padding:15px 50px;
    border-radius:10px;
    font-size:20px;
    cursor:pointer;
}

#app{
    display:none;
    padding:20px;
}

.titulo{
    text-align:center;
    color:#0d47a1;
    margin-bottom:20px;
}

.card{
    background:white;
    border-radius:20px;
    padding:25px;
    max-width:1200px;
    margin:auto;
    box-shadow:0 0 15px rgba(0,0,0,0.15);
}

.card h2{
    color:#0c7a2f;
    margin-bottom:15px;
}

.card p{
    line-height:1.8;
    font-size:18px;
}

.galeria{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:15px;
    max-width:1200px;
    margin:20px auto;
}

.galeria img{
    width:100%;
    height:250px;
    object-fit:cover;
    border-radius:15px;
}

.quiz{
    background:white;
    max-width:1200px;
    margin:auto;
    border-radius:20px;
    padding:25px;
    box-shadow:0 0 15px rgba(0,0,0,0.15);
}

.quiz h2{
    text-align:center;
    color:#0d47a1;
    margin-bottom:20px;
}

.perguntas{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:20px;
}

.pergunta{
    padding:10px;
}

.pergunta p{
    font-weight:bold;
    margin-bottom:10px;
}

.pergunta label{
    display:block;
    margin:8px 0;
}

.btn{
    text-align:center;
    margin-top:20px;
}

.btn button{
    background:#0d6efd;
    color:white;
    border:none;
    padding:15px 40px;
    border-radius:10px;
    cursor:pointer;
    font-size:18px;
}

#resultado{
    margin-top:20px;
    text-align:center;
    font-size:28px;
    color:green;
    font-weight:bold;
}

@media(max-width:768px){
    .perguntas{
        grid-template-columns:1fr;
    }

    #login h1{
        font-size:40px;
    }

    #login input{
        width:90%;
    }
}
</style>
</head>

<body>

<div id="login">

<h1>🌱 Raízes Verdes</h1>
<h2>Futuro Sustentável</h2>

<h3>Digite seu nome para entrar:</h3>
<br>

<input type="text" id="nome" placeholder="Digite seu nome">

<button onclick="entrar()">Entrar</button>

</div>

<div id="app">

<h1 class="titulo">
Bem-vindo(a), <span id="usuario"></span>! 🌱
</h1>

<div class="card">

<h2>Raízes Verdes: Futuro Sustentável</h2>

<p>
A agricultura é uma das atividades mais importantes para a sociedade, pois fornece alimentos, matérias-primas e gera empregos.
</p>

<br>

<p>
Para garantir um futuro melhor, é necessário produzir de forma responsável, respeitando o meio ambiente e preservando os recursos naturais.
</p>

<br>

<p>
O uso consciente da água, a preservação das florestas, a utilização de energias renováveis e a adoção de tecnologias modernas ajudam a aumentar a produção sem prejudicar a natureza.
</p>

<br>

<p>
O tema "Raízes Verdes: Futuro Sustentável" mostra que é possível unir desenvolvimento econômico, produção agrícola e preservação ambiental para construir um futuro melhor para todos.
</p>

</div>

<div class="galeria">

<img src="https://images.unsplash.com/photo-1464226184884-fa280b87c399?w=800">

<img src="https://images.unsplash.com/photo-1500382017468-9049fed747ef?w=800">

<img src="https://images.unsplash.com/photo-1501004318641-b39e6451bec6?w=800">

<img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?w=800">

</div>

<div class="quiz">

<h2>📝 Quiz - Raízes Verdes</h2>

<div class="perguntas">

<div class="pergunta">
<p>1. O que é sustentabilidade?</p>
<label><input type="radio" name="q1" value="1"> Produzir preservando os recursos naturais</label>
<label><input type="radio" name="q1" value="0"> Produzir sem cuidar do meio ambiente</label>
</div>

<div class="pergunta">
<p>2. Qual prática ajuda a conservar o solo?</p>
<label><input type="radio" name="q2" value="1"> Rotação de culturas</label>
<label><input type="radio" name="q2" value="0"> Queimadas frequentes</label>
</div>

<div class="pergunta">
<p>3. Qual recurso natural é essencial para a agricultura?</p>
<label><input type="radio" name="q3" value="1"> Água</label>
<label><input type="radio" name="q3" value="0"> Petróleo</label>
</div>

<div class="pergunta">
<p>4. O que ajuda a preservar as florestas?</p>
<label><input type="radio" name="q4" value="1"> Preservação de matas nativas</label>
<label><input type="radio" name="q4" value="0"> Desmatamento</label>
</div>

<div class="pergunta">
<p>5. O que é agricultura de precisão?</p>
<label><input type="radio" name="q5" value="1"> Uso de tecnologia para melhorar a produção</label>
<label><input type="radio" name="q5" value="0"> Plantar sem planejamento</label>
</div>

<div class="pergunta">
<p>6. Qual benefício da energia renovável?</p>
<label><input type="radio" name="q6" value="1"> Reduz impactos ambientais</label>
<label><input type="radio" name="q6" value="0"> Aumenta a poluição</label>
</div>

<div class="pergunta">
<p>7. Qual é uma fonte de energia limpa?</p>
<label><input type="radio" name="q7" value="1"> Energia solar</label>
<label><input type="radio" name="q7" value="0"> Carvão mineral</label>
</div>

<div class="pergunta">
<p>8. Por que devemos economizar água?</p>
<label><input type="radio" name="q8" value="1"> Porque é essencial para a vida</label>
<label><input type="radio" name="q8" value="0"> Porque não é importante</label>
</div>

<div class="pergunta">
<p>9. O que representa o tema Raízes Verdes?</p>
<label><input type="radio" name="q9" value="1"> Produção com responsabilidade ambiental</label>
<label><input type="radio" name="q9" value="0"> Produção sem preocupação ambiental</label>
</div>

<div class="pergunta">
<p>10. O que garante um futuro sustentável?</p>
<label><input type="radio" name="q10" value="1"> Equilíbrio entre produção e natureza</label>
<label><input type="radio" name="q10" value="0"> Exploração sem limites</label>
</div>

</div>

<div class="btn">
<button onclick="corrigirQuiz()">Ver Resultado</button>
</div>

<div id="resultado"></div>

</div>

</div>

<script>

function entrar(){

let nome = document.getElementById("nome").value;

if(nome==""){
alert("Digite seu nome!");
return;
}

document.getElementById("usuario").innerHTML = nome;

document.getElementById("login").style.display="none";
document.getElementById("app").style.display="block";

}

function corrigirQuiz(){

let pontos = 0;

for(let i=1;i<=10;i++){

let resposta =
document.querySelector('input[name="q'+i+'"]:checked');

if(resposta){
pontos += Number(resposta.value);
}

}

document.getElementById("resultado").innerHTML =
"🎉 Você acertou " + pontos + " de 10 perguntas!";

}

</script>

</body>
</html>