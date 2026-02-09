# For my pooks 
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Toosh 💕</title>
  <style>
    body{
      background:linear-gradient(135deg,#ff9a9e,#fad0c4);
      height:100vh;display:flex;justify-content:center;align-items:center;
      font-family:'Comic Sans MS',cursive;overflow:hidden;text-align:center
    }
    .card{
      background:#fff0f6;padding:35px;border-radius:25px;
      box-shadow:0 10px 30px rgba(0,0,0,.2);max-width:330px;z-index:2
    }
    h1{color:#ff4d88} p{color:#ff6fa5}
    img{width:150px;margin:15px 0}
    button{padding:12px 25px;font-size:16px;border-radius:20px;border:none;cursor:pointer;margin:10px}
    .yes{background:#ff4d88;color:#fff}
    .no{background:#fff;border:2px solid #ff4d88;color:#ff4d88;position:absolute}
    .heart{position:fixed;color:pink;font-size:20px;animation:float 5s linear infinite}
    @keyframes float{0%{transform:translateY(100vh);opacity:1}100%{transform:translateY(-10vh);opacity:0}}
    .sig{margin-top:10px;color:#ff6fa5;font-size:.9em}
  </style>
</head>
<body>

<audio autoplay loop>
  <source src="https://cdn.pixabay.com/audio/2022/03/15/audio_1c07f9b4c7.mp3" type="audio/mpeg">
</audio>

<div class="card">
  <h1>Toosh 💕</h1>
  <img src="https://media.giphy.com/media/MDJ9IbxxvDUQM/giphy.gif" alt="Cute Bear">
  <p>Will you be my Valentine? 💖</p>
  <button class="yes" onclick="go()">Yes 🧸</button>
  <button class="no" id="noBtn">No 🙃</button>
  <div class="sig">— Ozzie</div>
</div>

<script>
const noBtn=document.getElementById("noBtn");
noBtn.addEventListener("mouseover",()=>{
  noBtn.style.left=Math.random()*(window.innerWidth-120)+"px";
  noBtn.style.top=Math.random()*(window.innerHeight-60)+"px";
});
function go(){ window.location.href="yes.html"; }
setInterval(()=>{
  const h=document.createElement("div");h.className="heart";h.innerHTML="💖";
  h.style.left=Math.random()*100+"vw";h.style.fontSize=Math.random()*20+10+"px";
  document.body.appendChild(h);setTimeout(()=>h.remove(),5000);
},300);
</script>

</body>
</html>
