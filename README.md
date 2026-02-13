<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<title>Para ti, con todo cariño ❤️</title>
<style>
body {
    margin: 0;
    font-family: Georgia, serif;
    background: linear-gradient(135deg, #ffb6c1, #ffe4e1);
    overflow: hidden;
}

.screen {
    display: none;
    height: 100vh;
    width: 100vw;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    text-align: center;
    padding: 50px 40px 100px;
    box-sizing: border-box;
}

.active {
    display: flex;
}

h1 {
    color: #b30047;
    margin-bottom: 20px;
}

p {
    max-width: 800px;
    font-size: 1.1em;
    color: #5a0033;
    background: rgba(255,255,255,0.85);
    padding: 22px;
    border-radius: 15px;
    box-shadow: 0 0 10px rgba(0,0,0,0.1);
    line-height: 1.6;
}

button {
    margin-top: 20px;
    padding: 10px 22px;
    border: none;
    border-radius: 20px;
    background: #ff4d88;
    color: white;
    font-size: 1em;
    cursor: pointer;
}

button:hover {
    background: #e6005c;
}

.music-btn {
    position: fixed;
    bottom: 15px;
    right: 15px;
    background: #ff4d88;
    padding: 10px 15px;
    border-radius: 50px;
    z-index: 999;
}

.heart {
    position: fixed;
    bottom: -20px;
    color: rgba(255, 0, 80, 0.5);
    font-size: 20px;
    animation: float 10s linear infinite;
}

@keyframes float {
    from { transform: translateY(0); opacity: 1; }
    to { transform: translateY(-110vh); opacity: 0; }
}
</style>
</head>
<body>

<audio id="bgMusic" autoplay loop>
    <source src="musica.mp3" type="audio/mpeg">
</audio>

<button class="music-btn" onclick="toggleMusic()">🎵 Música</button>

<div id="start" class="screen active">
    <h1>Para ti, con todo cariño ❤️</h1>
    <button onclick="goTo('paths')">Comenzar</button>
</div>

<div id="paths" class="screen">
    <h1>Elige un camino ✨</h1>
    <button onclick="goTo('p1')">Leer la carta</button>
    <button onclick="goTo('soft')">Un mensajito aparte</button>
</div>

<div id="p1" class="screen"><p>Para el día de hoy, 14 de febrero, quise escribirte una carta digital, ya que actualmente no puedo obsequiarte flores o algún otro detalle de manera presencial. Por eso decidí escribir esto como un pequeño detalle para expresarte lo que significas para mí.</p><button onclick="goTo('p2')">Siguiente</button></div>

<div id="p2" class="screen"><p>Tú ya sabes mis intenciones contigo. La verdad es que te considero una gran mujer, independientemente de que me lleves algunos años de más. Soy muy consciente de todo lo que ha pasado en estos últimos años; aun así, quiero arriesgarme contigo. Sé que suena loco y sé todo lo que puedas pensar, pero en realidad quiero que se llegue a dar algo. Ya te he aclarado que mi interés hacia ti no va por cosas materiales; al contrario, mi interés en ti es genuino y quiero construir algo bonito contigo.</p><button onclick="goTo('p3')">Siguiente</button></div>

<div id="p3" class="screen"><p>No te quiero para un momento ni mucho menos para distraerme; te quiero para abrazarte, reírnos, amarnos, pelearnos, enojarnos, pero todo contigo; corregir errores juntos, verte crecer y cumplir tus metas y sueños. No me importa qué tan difícil sea el camino; siempre seríamos tú y yo contra el mundo. También quiero que llegues a confiar plenamente en mí, porque jamás trataría de romper algo tan valioso.</p><button onclick="goTo('p4')">Siguiente</button></div>

<div id="p4" class="screen"><p>No me importa que me tome el tiempo que sea lograr todo eso; prefiero ir a pasos de tortuga antes que forzar algo, porque algo forzado jamás funciona. Contigo trato de ser lo más transparente posible, sin mentiras ni segundas intenciones. Sé que a veces puedo sonar ingenuo al decir cosas así, porque aún me falta avanzar un poco más en la vida, pero no creo que esté mal expresar lo que siento.</p><button onclick="goTo('p5')">Siguiente</button></div>

<div id="p5" class="screen"><p>Después de la etapa en la que me comporté como un insensible contigo, recuerdo que me dijiste que me demostrarías que habías entendido todo. Confieso que por un instante dudé de eso, tal vez por el enojo que tenía, pero hoy veo que me equivoqué al pensar mal de ti. Antes te dije que me sentía orgulloso de ti cuando dejaste de sufrir y te enfocaste en tu hijo, porque siempre te he considerado una gran mamá y lo sostengo.</p><button onclick="goTo('p6')">Siguiente</button></div>

<div id="p6" class="screen"><p>Ahora, saber todo lo que has logrado me llena aún más de orgullo, porque lo que me dijiste que habías entendido era verdad y era algo que yo quería que lograras. De verdad me da mucha felicidad ver todo lo que has conseguido.</p><button onclick="goTo('p7')">Siguiente</button></div>

<div id="p7" class="screen"><p>Todo lo que he dicho en esta “carta” se queda corto a todo lo que quisiera expresar, porque hay cosas que no se pueden explicar con palabras. Para mí eres alguien muy especial, alguien a quien le puedo ser leal por el resto de mi vida; alguien por quien puedo poner en riesgo todo porque sé que valdría totalmente la pena. Lo que digo no es labia: es lo que realmente siento, y por eso quiero arriesgarme a conquistarte.</p><button onclick="goTo('p8')">Siguiente</button></div>

<div id="p8" class="screen"><p>Antes te dije que no competiría con los posibles pretendientes que tuvieras, que me enfocaría en lo que yo hago. Sé que no la tengo fácil, pero considero que hasta el momento no lo he hecho mal.</p><button onclick="goTo('p9')">Siguiente</button></div>

<div id="p9" class="screen"><p>Pongo mi fe en Dios en que todo irá bien. Hace poco leí un pasaje bíblico; no lo pondré aquí porque mi intención no es predicarte nada, pero sí decirte dónde está por si quieres leerlo: 1 Corintios 13:4-7. Me da pena decir algo tan cursi, pero lo diré directo: creo que podría llegar a amarte de esa forma si llegase a enamorarme de ti.</p><button onclick="goTo('p10')">Siguiente</button></div>

<div id="p10" class="screen"><p>Por la manera en que soy como persona, sé que así lo haría, y me gustaría que lo leyeras para que entiendas a qué me refiero. Algunas de las cosas que he dicho aquí ya las has leído en los videos que te he mandado. No los enviaba solo por el momento; también los tomaba como referencia para escribir todo esto.</p><button onclick="goTo('p11')">Siguiente</button></div>

<div id="p11" class="screen"><p>Y sabes algo: no me arrepiento de nada de lo que te he dicho. Todo sale de mi corazón. Aprecio profundamente que seas parte de mi vida; tu compañía me llena de felicidad, aunque sea a través de una pantalla.</p><button onclick="goTo('p12')">Siguiente</button></div>

<div id="p12" class="screen"><p>Me gustas, Jenifer, y ya te lo he dicho antes. Ya te mencioné que me refiero más a lo empírico, pero claro que físicamente también me atraes porque eres muy hermosa; aun así, eso es superficial. Quiero hacerte sentir algo nuevo, algo bonito donde te sientas cuidada, querida y, sobre todo, en paz.</p><button onclick="goTo('p13')">Siguiente</button></div>

<div id="p13" class="screen"><p>Yo aprenderé a quererte bien, y quiero lograr que pienses lo mismo de mí. Tomará tiempo, pero sé que valdrá totalmente la pena.</p><button onclick="goTo('p14')">Siguiente</button></div>

<div id="p14" class="screen"><p>No te escribo esto para que me respondas algo ahora mismo ni para que sientas que tienes que decidir algo; solo quería ser honesto contigo con lo que siento hoy.</p><button onclick="goTo('p15')">Siguiente</button></div>

<div id="p15" class="screen"><p>No sé qué nos depare el tiempo, pero sí sé que hoy me nace intentar construir algo bonito contigo, con calma y con el corazón en el lugar correcto. Pongo mi fe en Dios en que todo se dará como tenga que darse; yo, por mi parte, quiero intentar hacer las cosas bien contigo.</p><button onclick="goTo('paths')">Volver al inicio</button></div>

<div id="soft" class="screen">
<p>
No tienes que sentir nada que no te nazca.  
No tienes que responder nada que no te salga.  
Esto es solo algo que quise hacer porque me nace tener un detalle contigo.  
<br><br>
Esto no es para apurarte ni para que decidas algo.  
Es solo un recordatorio bonito de que alguien te aprecia, te respeta y quiere hacer las cosas con calma y con el corazón en el lugar correcto.
</p>
<button onclick="goTo('paths')">Volver al inicio</button>
</div>

<script>
function goTo(id) {
    document.querySelectorAll('.screen').forEach(s => s.classList.remove('active'));
    document.getElementById(id).classList.add('active');
}

function toggleMusic() {
    const music = document.getElementById("bgMusic");
    if (music.paused) music.play();
    else music.pause();
}

function createHeart() {
    const heart = document.createElement("div");
    heart.className = "heart";
    heart.innerHTML = "❤️";
    heart.style.left = Math.random() * 100 + "vw";
    heart.style.animationDuration = (6 + Math.random() * 6) + "s";
    document.body.appendChild(heart);
    setTimeout(() => heart.remove(), 12000);
}

setInterval(createHeart, 700);
</script>

</body>
</html>
