# dark
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Para Daisy 🖤</title>
<style>
*{
  box-sizing:border-box;
  margin:0;
  padding:0;
}
html{
  scroll-behavior:smooth;
}
body{
  font-family:Georgia,"Times New Roman",serif;
  background:#030303;
  color:#eee;
  overflow-x:hidden;
}
/* FUNDO */
body::before{
  content:"";
  position:fixed;
  inset:0;
  z-index:-3;
  background:
    radial-gradient(circle at 50% 15%,rgba(110,0,0,.25),transparent 38%),
    radial-gradient(circle at 20% 80%,rgba(80,0,0,.12),transparent 35%),
    linear-gradient(180deg,#020202,#090303,#020202);
}
body::after{
  content:"";
  position:fixed;
  inset:0;
  z-index:-2;
  pointer-events:none;
  background:
    repeating-linear-gradient(
      115deg,
      transparent 0px,
      transparent 80px,
      rgba(255,255,255,.012) 81px,
      transparent 82px
    );
}
/* PARTÍCULAS */
.particle{
  position:fixed;
  bottom:-20px;
  color:#720000;
  font-size:18px;
  opacity:0;
  animation:float 9s linear infinite;
  pointer-events:none;
  z-index:2;
}
.p1{left:8%;animation-delay:0s}
.p2{left:25%;animation-delay:3s}
.p3{left:47%;animation-delay:6s}
.p4{left:70%;animation-delay:2s}
.p5{left:90%;animation-delay:4s}
@keyframes float{
  0%{
    transform:translateY(0) scale(.7);
    opacity:0;
  }
  15%{
    opacity:.5;
  }
  100%{
    transform:translateY(-110vh) scale(1.4) rotate(25deg);
    opacity:0;
  }
}
/* GERAL */
section{
  min-height:100vh;
  padding:80px 20px;
  display:flex;
  align-items:center;
  justify-content:center;
  position:relative;
}
.container{
  width:min(900px,100%);
  margin:auto;
  text-align:center;
}
.small{
  text-transform:uppercase;
  letter-spacing:5px;
  font-size:11px;
  color:#777;
  margin-bottom:28px;
}
.title{
  font-size:clamp(34px,8vw,62px);
  margin-bottom:30px;
  line-height:1.15;
}
.text{
  max-width:720px;
  margin:auto;
  color:#bbb;
  font-size:19px;
  line-height:2;
}
/* GHOSTFACE */
#inicio{
  background:
    radial-gradient(
      circle at center,
      rgba(120,0,0,.25),
      transparent 48%
    );
}
.ghost{
  width:145px;
  height:190px;
  background:#ddd;
  margin:0 auto 45px;
  border-radius:48% 48% 42% 42%;
  position:relative;
  box-shadow:
    0 0 45px rgba(255,255,255,.06),
    0 30px 80px #000;
}
.ghost:before,
.ghost:after{
  content:"";
  position:absolute;
  top:43px;
  width:31px;
  height:58px;
  background:#050505;
  border-radius:50%;
}
.ghost:before{
  left:33px;
  transform:rotate(18deg);
}
.ghost:after{
  right:33px;
  transform:rotate(-18deg);
}
.mouth{
  position:absolute;
  width:58px;
  height:75px;
  background:#050505;
  border-radius:50%;
  left:50%;
  bottom:16px;
  transform:translateX(-50%);
}
h1{
  font-size:clamp(65px,17vw,135px);
  line-height:.85;
  color:#eee;
  text-shadow:0 0 40px rgba(120,0,0,.35);
  margin-bottom:30px;
}
.red{
  color:#9b0000;
}
.subtitle{
  max-width:650px;
  margin:auto;
  font-size:21px;
  line-height:1.8;
  color:#aaa;
}
.scroll{
  margin-top:55px;
  color:#666;
  font-size:13px;
  animation:pulse 2s infinite;
}
@keyframes pulse{
  50%{
    opacity:.25;
  }
}
/* CARDS */
.card,
.love-card{
  background:rgba(255,255,255,.025);
  border:1px solid rgba(150,0,0,.20);
  border-radius:28px;
  padding:45px 30px;
  box-shadow:
    0 25px 80px rgba(0,0,0,.7),
    inset 0 0 30px rgba(120,0,0,.025);
  backdrop-filter:blur(8px);
}
.card p{
  font-size:20px;
  line-height:2;
  color:#ccc;
  margin-bottom:25px;
}
.highlight{
  color:#a60000;
  font-weight:bold;
}
/* HISTÓRIA */
#historia{
  background:
    linear-gradient(
      180deg,
      #030303,
      #0b0303,
      #030303
    );
}
/* DAISY */
#daisy{
  background:
    radial-gradient(
      circle at center,
      rgba(100,0,0,.16),
      transparent 60%
    );
}
.big{
  font-size:clamp(32px,8vw,67px);
  line-height:1.3;
  font-weight:bold;
}
.big span{
  color:#a40000;
}
.line{
  width:75px;
  height:2px;
  background:#850000;
  margin:35px auto;
}
/* ENCONTRO */
#encontro{
  background:#020202;
}
.heart{
  font-size:75px;
  margin-bottom:25px;
  color:#8d0000;
  text-shadow:0 0 35px rgba(150,0,0,.4);
}
.meeting{
  font-size:clamp(26px,6vw,43px);
  line-height:1.6;
  color:#ddd;
}
.meeting span{
  color:#a00000;
}
/* DECLARAÇÃO */
#declaracao-amor{
  background:
    radial-gradient(
      circle at center,
      rgba(120,0,0,.20),
      transparent 60%
    ),
    #030303;
}
.love-card{
  max-width:800px;
  margin:auto;
}
.love-card p{
  font-size:20px;
  line-height:2;
  color:#cfcfcf;
  margin-bottom:28px;
}
.love-divider{
  color:#920000;
  font-size:28px;
  margin:35px 0;
  text-shadow:
    0 0 20px rgba(150,0,0,.5);
}
.love-highlight{
  color:#e5e5e5 !important;
}
.big-love{
  font-size:clamp(27px,6vw,42px) !important;
  font-weight:bold;
  color:#a80000 !important;
  text-shadow:
    0 0 25px rgba(150,0,0,.25);
}
.signature-love{
  margin-top:45px;
  font-size:28px;
  color:#ddd;
  font-style:italic;
}
/* DECLARAÇÃO EXTRA */
#declaracao{
  background:
    radial-gradient(
      circle at center,
      rgba(100,0,0,.15),
      transparent 60%
    );
}
.quote{
  font-size:clamp(22px,5vw,32px);
  line-height:1.75;
  color:#e6e6e6;
  margin:30px auto;
}
/* FINAL */
#final{
  min-height:90vh;
  background:
    radial-gradient(
      circle at center,
      rgba(120,0,0,.3),
      transparent 55%
    ),
    #020202;
}
.final{
  font-size:clamp(38px,9vw,76px);
  font-weight:bold;
  line-height:1.25;
}
.final span{
  color:#a00000;
}
.forever{
  margin-top:35px;
  color:#999;
  font-size:19px;
  line-height:1.9;
}
footer{
  padding:35px 20px;
  background:#010101;
  color:#555;
  text-align:center;
  font-size:12px;
  letter-spacing:2px;
}
/* CELULAR */
@media(max-width:600px){
  .card,
  .love-card{
    padding:32px 20px;
  }
  .card p,
  .love-card p{
    font-size:18px;
    line-height:1.9;
  }
  .ghost{
    transform:scale(.75);
    margin-bottom:15px;
  }
}
</style>
</head>
<body>
<!-- PARTÍCULAS -->
<div class="particle p1">♥</div>
<div class="particle p2">♥</div>
<div class="particle p3">♥</div>
<div class="particle p4">♥</div>
<div class="particle p5">♥</div>
<!-- CAPA -->
<section id="inicio">
<div class="container">
<div class="ghost">
  <div class="mouth"></div>
</div>
<div class="small">
Uma coisa que eu queria te dizer
</div>
<h1>
Daisy<span class="red">.</span>
</h1>
<p class="subtitle">
Talvez você ainda não saiba o tamanho do espaço
que conseguiu ocupar dentro de mim.
</p>
<div class="scroll">
↓ continua ↓
</div>
</div>
</section>
<!-- HISTÓRIA -->
<section id="historia">
<div class="container">
<div class="small">
Entre nós dois
</div>
<h2 class="title">
Ainda existe muito para acontecer.
</h2>
<div class="card">
<p>
A gente ainda nem teve a chance de se olhar
de perto, de sentar um ao lado do outro
ou simplesmente passar algumas horas juntos.
</p>
<p>
E mesmo assim, de alguma forma,
você conseguiu se tornar alguém importante
para mim.
</p>
<p>
Talvez seja estranho.
Talvez seja loucura.
Mas talvez algumas histórias simplesmente
comecem antes do primeiro encontro.
</p>
<p>
E eu não quero apressar o que ainda precisa
acontecer.
</p>
<p>
Quero descobrir você aos poucos,
até chegar o dia em que finalmente
vou poder olhar nos seus olhos e pensar:
</p>
<p>
<span class="highlight">
"Então era você."
</span>
</p>
</div>
</div>
</section>
<!-- DAISY -->
<section id="daisy">
<div class="container">
<div class="small">
Para você
</div>
<div class="big">
Daisy,<br>
você já é uma parte<br>
<span>da minha história.</span>
</div>
<div class="line"></div>
<p class="text">
Eu gosto desse nosso jeito meio estranho,
intenso e difícil de explicar.
<br><br>
Gosto das conversas,
das provocações,
das noites falando besteira
e daqueles momentos em que parece
que o resto do mundo simplesmente desaparece.
<br><br>
E talvez seja exatamente isso
que torna tudo tão especial.
</p>
</div>
</section>
<!-- ENCONTRO -->
<section id="encontro">
<div class="container">
<div class="heart">
♥
</div>
<div class="small">
O dia que ainda vai chegar
</div>
<div class="meeting">
Eu ainda não sei exatamente
como vai ser o nosso primeiro encontro.
<br><br>
Mas sei que em algum momento
a distância vai deixar de existir.
<br><br>
E quando eu finalmente estiver
na sua frente...
<br><br>
<span>
eu quero lembrar desse momento
para o resto da minha vida.
</span>
</div>
</div>
</section>
<!-- DECLARAÇÃO DE AMOR -->
<section id="declaracao-amor">
<div class="container">
<div class="small">
O que eu sinto por você
</div>
<h2 class="title">
Daisy, eu amo você. 🖤
</h2>
<div class="love-card">
<p>
Eu nem sei explicar direito como alguém que ainda nem
esteve fisicamente ao meu lado conseguiu se tornar tão
importante para mim.
</p>
<p>
Mas você conseguiu.
</p>
<p>
Eu amo cada detalhe seu. Amo seu jeito, sua voz,
suas manias, suas provocações, seu sorriso e até aqueles
pequenos detalhes que talvez você nem perceba,
mas que eu reparo.
</p>
<p>
Para mim, você é perfeita.
Não porque não tenha defeitos, mas porque até aquilo
que você chama de defeito faz parte da garota que
eu aprendi a amar.
</p>
<p>
Eu amo a forma como você consegue mudar completamente
o meu dia só com uma conversa.
Amo quando você me faz sorrir sem perceber.
Amo quando a gente fica conversando por horas
e parece que o tempo simplesmente desaparece.
</p>
<div class="love-divider">♥</div>
<p>
E talvez a parte mais bonita seja saber que ainda existe
tanto de você que eu quero conhecer.
</p>
<p>
Eu ainda não pude olhar nos seus olhos de perto.
Ainda não pude te abraçar.
Ainda não pude segurar sua mão.
</p>
<p>
Mas mesmo assim, existe algo dentro de mim
que já escolheu você.
</p>
<p class="love-highlight">
E quando finalmente chegar o dia em que eu estiver
diante de você, eu quero te olhar e lembrar de todas
as noites, todas as conversas e todos os sentimentos
que nos trouxeram até aquele momento.
</p>
<p>
Daisy, eu amo você.
</p>
<p>
E se eu pudesse te mostrar o tamanho desse amor
em vez de tentar explicar com palavras,
talvez você finalmente entendesse por que,
para mim, você é tão especial.
</p>
<p>
Você não precisa ser perfeita para o mundo.
</p>
<p class="love-highlight big-love">
Para mim, basta ser você.
</p>
<p>
Porque foi exatamente essa garota que eu conheci,
essa garota que me conquistou e essa garota que
eu quero continuar descobrindo.
</p>
<div class="signature-love">
Minha Daisy. 🖤
</div>
</div>
</div>
</section>
<!-- DECLARAÇÃO MAIS INTENSA -->
<section id="declaracao">
<div class="container">
<div class="small">
Agora presta atenção
</div>
<h2 class="title">
Eu escolheria você.
</h2>
<div class="card">
<p class="quote">
Eu não quero uma história perfeita.
</p>
<p class="quote">
Quero uma história verdadeira.
Daquelas que têm noites boas,
dias complicados, risadas,
saudade e vontade de ficar.
</p>
<p class="quote">
Quero conhecer cada versão sua.
A menina que ri de tudo,
a que fica quieta,
a que provoca,
a que sente demais
e até aquela que tenta esconder
quando está com saudade.
</p>
<p class="quote">
E quando finalmente estivermos
frente a frente,
eu quero que você saiba
que eu esperei por aquele momento
sem deixar de escolher você.
</p>
<p class="quote">
Porque, no meio de tanta gente,
foi você que despertou
essa vontade em mim.
</p>
<p class="quote">
E se isso é loucura...
<br><br>
<span class="highlight">
então deixa a gente ser louco junto.
</span>
</p>
</div>
</div>
</section>
<!-- FINAL -->
<section id="final">
<div class="container">
<div class="final">
Daisy,<br>
<span>
eu ainda vou te encontrar.
</span>
</div>
<p class="forever">
E quando esse dia chegar,<br>
eu quero olhar para você
e lembrar de tudo que começou
antes daquele momento.
</p>
<p class="forever">
Até lá...
<br><br>
fica aqui.
<br>
Comigo.
</p>
<p class="forever">
🖤
<br><br>
<strong>
Nossa história ainda está começando.
</strong>
</p>
</div>
</section>
<footer>
Feito especialmente para Daisy 🖤
</footer>
</body>
</html>