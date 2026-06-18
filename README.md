# Day.com
Dayrelis publico
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>💖 Palabras de Dios para Dayrelis 💖</title>
<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Segoe UI',sans-serif;
}
body{
    min-height:100vh;
    background:linear-gradient(135deg,#ffb6d9,#d7b8ff,#fff0c9);
    overflow-x:hidden;
    color:#fff;
}
.estrellas{
    position:fixed;
    width:100%;
    height:100%;
    top:0;
    left:0;
    z-index:-1;
}
.estrella{
    position:absolute;
    width:3px;
    height:3px;
    background:white;
    border-radius:50%;
    animation:brillar 2s infinite alternate;
}
@keyframes brillar{
    from{opacity:.2;}
    to{opacity:1;}
}
.container{
    max-width:900px;
    margin:auto;
    padding:20px;
}
.hero{
    text-align:center;
    padding:50px 20px;
}
.hero h1{
    font-size:3rem;
    text-shadow:0 0 20px rgba(255,255,255,.7);
}
.hero p{
    margin-top:15px;
    font-size:1.2rem;
}
.card{
    background:rgba(255,255,255,.15);
    backdrop-filter:blur(10px);
    border-radius:25px;
    padding:25px;
    margin:20px 0;
    box-shadow:0 10px 25px rgba(0,0,0,.2);
}
h2{
    margin-bottom:15px;
}
select,button{
    width:100%;
    padding:15px;
    border:none;
    border-radius:15px;
    margin-top:10px;
    font-size:1rem;
}
button{
    cursor:pointer;
    background:#ff4fa3;
    color:white;
    font-weight:bold;
}
button:hover{
    transform:scale(1.03);
}
.resultado{
    margin-top:20px;
    font-size:1.1rem;
    line-height:1.8;
}
.versiculo{
    font-style:italic;
    margin-top:15px;
}
.razon{
    text-align:center;
    font-size:1.2rem;
    margin-top:20px;
}
footer{
    text-align:center;
    padding:30px;
}
</style>
</head>
<body>
<div class="estrellas" id="estrellas"></div>
<div class="container">
<div class="hero">
<h1>💖 Palabras de Dios para Dayrelis 💖</h1>
<p>
Un lugar especial para que encuentres amor, paz,
esperanza y palabras hermosas de Dios cuando más las necesites.
🌷✨
</p>
</div>
<div class="card">
<h2>🌸 ¿Cómo te sientes hoy?</h2>
<select id="emocion">
<option value="">Selecciona una opción</option>
<option value="triste">😢 Triste</option>
<option value="feliz">😊 Feliz</option>
<option value="preocupada">😰 Preocupada</option>
<option value="sola">😔 Sola</option>
<option value="fortaleza">🙏 Necesito fuerza</option>
<option value="amada">💖 Quiero sentirme amada</option>
<option value="esperanza">🌈 Necesito esperanza</option>
</select>
<button onclick="mostrarMensaje()">
📖 Mostrar Palabra de Dios
</button>
<div id="resultado" class="resultado"></div>
</div>
<div class="card">
<h2>💌 Carta Especial</h2>
<p>
Dayrelis, recuerda siempre que eres una mujer maravillosa,
valiosa y amada por Dios.
Cuando tengas un día difícil,
entra aquí y permite que estas palabras llenen tu corazón
de paz, amor y esperanza.
Nunca olvides que Dios tiene planes hermosos para tu vida
y que tu sonrisa ilumina a quienes te rodean. ❤️
</p>
</div>
<div class="card">
<h2>💝 Razones por las que eres especial</h2>
<button onclick="razonAleatoria()">
✨ Mostrar una razón
</button>
<div id="razon" class="razon"></div>
</div>
</div>
<footer>
🌷 Hecho con amor para Dayrelis 💖
</footer>
<script>
const mensajes = {
triste:{
versiculo:"Cercano está Jehová a los quebrantados de corazón. — Salmos 34:18",
texto:"Aunque hoy te sientas triste, Dios está contigo y nunca te abandonará."
},
feliz:{
versiculo:"Este es el día que hizo Jehová; nos gozaremos y alegraremos en él. — Salmos 118:24",
texto:"Disfruta tu alegría y agradece a Dios por cada bendición."
},
preocupada:{
versiculo:"Echa sobre Jehová tu carga y él te sustentará. — Salmos 55:22",
texto:"No cargues sola tus preocupaciones. Dios pelea tus batallas."
},
sola:{
versiculo:"No te dejaré ni te desampararé. — Hebreos 13:5",
texto:"Nunca estás sola. Dios camina contigo en todo momento."
},
fortaleza:{
versiculo:"Todo lo puedo en Cristo que me fortalece. — Filipenses 4:13",
texto:"Eres más fuerte de lo que imaginas porque Dios está contigo."
},
amada:{
versiculo:"Con amor eterno te he amado. — Jeremías 31:3",
texto:"Eres profundamente amada por Dios y muy especial."
},
esperanza:{
versiculo:"Porque yo sé los planes que tengo para vosotros. — Jeremías 29:11",
texto:"Hay cosas hermosas esperándote más adelante."
}
};
function mostrarMensaje(){
let emocion = document.getElementById("emocion").value;
if(!emocion){
return;
}
document.getElementById("resultado").innerHTML=
`
<p>${mensajes[emocion].texto}</p>
<p class="versiculo">
📖 ${mensajes[emocion].versiculo}
</p>
`;
}
const razones = [
"Porque tu sonrisa ilumina los días.",
"Porque tienes un corazón hermoso.",
"Porque eres única.",
"Porque Dios te creó especial.",
"Porque inspiras a quienes te rodean.",
"Porque eres valiente.",
"Porque eres amable.",
"Porque tu presencia trae alegría.",
"Porque tienes un alma hermosa.",
"Porque haces del mundo un lugar mejor.",
"Porque mereces ser feliz.",
"Porque tu forma de ser es maravillosa.",
"Porque eres un regalo de Dios.",
"Porque nunca dejas de intentarlo.",
"Porque tienes una luz especial.",
"Porque eres increíble.",
"Porque tu bondad destaca.",
"Porque haces sonreír a otros.",
"Porque eres auténtica.",
"Porque eres valiosa."
];
function razonAleatoria(){
const numero =
Math.floor(Math.random()*razones.length);
document.getElementById("razon").innerHTML =
"💖 " + razones[numero];
}
for(let i=0;i<120;i++){
let estrella=document.createElement("div");
estrella.classList.add("estrella");
estrella.style.left=Math.random()*100+"%";
estrella.style.top=Math.random()*100+"%";
estrella.style.animationDuration=
(Math.random()*3+1)+"s";
document.getElementById("estrellas")
.appendChild(estrella);
}
</script>
</body>
</html>