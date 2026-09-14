<!DOCTYPE html>
<html lang="hi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>Rohit AI</title>

<style>
*{box-sizing:border-box}
body{
 margin:0;font-family:Arial,sans-serif;
 background:linear-gradient(135deg,#111827,#312e81,#581c87);
 color:white;min-height:100vh
}
.app{max-width:600px;margin:auto;padding:20px}
.logo{text-align:center;font-size:36px;font-weight:bold;margin-top:25px}
.tag{text-align:center;opacity:.8;margin:8px 0 25px}
.card{
 background:rgba(255,255,255,.1);
 border:1px solid rgba(255,255,255,.15);
 border-radius:20px;padding:18px;margin-bottom:16px
}
textarea{
 width:100%;height:120px;border:0;border-radius:14px;
 padding:15px;font-size:16px;outline:0
}
button{
 width:100%;border:0;border-radius:14px;
 padding:14px;margin-top:12px;
 font-size:16px;font-weight:bold;
 background:white;color:#312e81
}
button:active{transform:scale(.98)}
.features{
 display:grid;grid-template-columns:1fr 1fr;gap:10px
}
.feature{
 background:rgba(255,255,255,.08);
 padding:15px;border-radius:14px;text-align:center
}
#reply{line-height:1.6;white-space:pre-wrap}
</style>
</head>

<body>
<div class="app">

<div class="logo">🤖 Rohit AI</div>
<div class="tag">Your Personal AI Assistant 🚀</div>

<div class="card">
<h3>💬 AI Chat</h3>

<textarea id="question"
placeholder="Rohit AI se kuch bhi poochho..."></textarea>

<button onclick="askAI()">✨ Ask Rohit AI</button>
</div>

<div class="card">
<h3>🎯 Rohit Mode</h3>
<p>Apna goal likho aur AI ke saath step-by-step plan banao.</p>

<button onclick="rohitMode()">🚀 Start Rohit Mode</button>
</div>

<div class="card">
<h3>⚡ Features</h3>

<div class="features">
<div class="feature">💬 AI Chat</div>
<div class="feature">🎨 Photo Help</div>
<div class="feature">🎬 Reel Scripts</div>
<div class="feature">🎙️ Voice</div>
<div class="feature">📷 Image AI</div>
<div class="feature">🧠 Memory</div>
</div>
</div>

<div class="card">
<h3>🤖 Response</h3>
<div id="reply">Rohit AI ready hai... 🔥</div>
</div>

</div>

<script>

function askAI(){

let q=document.getElementById("question").value.trim();
let reply=document.getElementById("reply");

if(!q){
reply.textContent="Bhai pehle question likho 😄";
return;
}

reply.textContent=
"🔥 Rohit AI Prototype\n\n"+
"Tumne poocha:\n"+q+
"\n\nAI engine abhi connect karna baaki hai. 🚀";

}

function rohitMode(){

let goal=prompt("🎯 Apna goal likho:");

if(!goal)return;

document.getElementById("reply").textContent=
"🚀 ROHIT MODE\n\n"+
"Goal: "+goal+
"\n\n"+
"1️⃣ Goal clear karo\n"+
"2️⃣ Goal ko chhote tasks mein divide karo\n"+
"3️⃣ Daily progress check karo\n"+
"4️⃣ Feedback ke according plan improve karo\n\n"+
"🔥 Rohit AI tumhare saath hai!";

}

</script>

</body>
</html>
