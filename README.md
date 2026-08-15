<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Résultats — Yaz Okulu 2026 — Français A1</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Baloo+2:wght@500;600;700;800&family=Nunito:wght@400;600;700;800&display=swap" rel="stylesheet">
<style>
  :root{
    --cream:#FFFBF2;
    --cream-2:#FFF3DE;
    --sky:#29ABE2;
    --sky-deep:#1C8FC2;
    --coral:#FF6F59;
    --yellow:#FFC857;
    --green:#4CAF7D;
    --plum:#2E2540;
    --plum-soft:#5A4E72;
    --gold:#E6A817;
  }
  *{box-sizing:border-box;}
  body{
    margin:0;
    min-height:100vh;
    font-family:'Nunito',sans-serif;
    color:var(--plum);
    background:
      radial-gradient(circle at 12% 15%, rgba(41,171,226,0.16), transparent 40%),
      radial-gradient(circle at 88% 10%, rgba(255,200,87,0.22), transparent 38%),
      radial-gradient(circle at 85% 85%, rgba(76,175,125,0.16), transparent 40%),
      radial-gradient(circle at 10% 88%, rgba(255,111,89,0.14), transparent 38%),
      var(--cream);
    display:flex;
    align-items:center;
    justify-content:center;
    padding:28px 16px;
    overflow-x:hidden;
  }
  .stage{width:100%;max-width:620px;}

  /* ---------- decorative sky trail ---------- */
  .trail{position:fixed;inset:0;pointer-events:none;z-index:0;}
  .dot{position:absolute;border-radius:50%;opacity:.55;}

  /* ---------- header eyebrow ---------- */
  .eyebrow{
    text-align:center;
    font-family:'Baloo 2',sans-serif;
    font-weight:700;
    letter-spacing:.08em;
    color:var(--sky-deep);
    font-size:14px;
    text-transform:uppercase;
    margin-bottom:10px;
  }

  /* ---------- passport card ---------- */
  .passport{
    position:relative;
    z-index:1;
    background:linear-gradient(160deg,#ffffff, var(--cream-2));
    border-radius:28px;
    box-shadow:0 24px 60px -20px rgba(46,37,64,.35), 0 2px 0 rgba(255,255,255,.6) inset;
    border:3px solid var(--plum);
    padding:34px 28px 30px;
    animation:riseIn .7s cubic-bezier(.2,.9,.25,1) both;
  }
  @keyframes riseIn{from{opacity:0;transform:translateY(24px) scale(.97);}to{opacity:1;transform:translateY(0) scale(1);}}

  .badge-row{display:flex;justify-content:center;margin-bottom:6px;}
  .plane{font-size:30px;display:inline-block;animation:fly 3.2s ease-in-out infinite;}
  @keyframes fly{0%,100%{transform:translateX(0) rotate(0deg);}50%{transform:translateX(6px) rotate(6deg);}}

  h1.title{
    font-family:'Baloo 2',sans-serif;
    font-weight:800;
    text-align:center;
    font-size:clamp(26px,6vw,34px);
    margin:4px 0 6px;
    color:var(--plum);
  }
  .subtitle{
    text-align:center;
    font-weight:700;
    color:var(--sky-deep);
    font-size:15px;
    margin-bottom:22px;
  }

  .prof-card{
    background:var(--plum);
    color:#fff;
    border-radius:18px;
    padding:16px 18px;
    display:flex;
    align-items:center;
    gap:14px;
    margin-bottom:22px;
    box-shadow:0 10px 24px -12px rgba(46,37,64,.55);
  }
  .prof-avatar{
    width:52px;height:52px;flex:0 0 52px;
    border-radius:14px;
    background:linear-gradient(135deg,var(--sky),var(--green));
    display:flex;align-items:center;justify-content:center;
    font-family:'Baloo 2',sans-serif;font-weight:800;font-size:20px;
  }
  .prof-text{line-height:1.35;}
  .prof-text .name{font-family:'Baloo 2',sans-serif;font-weight:700;font-size:17px;}
  .prof-text .meta{font-size:13.5px;color:#D9D2EA;font-weight:600;}

  .lead{
    text-align:center;
    font-size:15px;
    line-height:1.55;
    color:var(--plum-soft);
    font-weight:600;
    margin-bottom:24px;
  }

  /* ---------- code entry ---------- */
  .code-form{display:flex;flex-direction:column;gap:14px;align-items:center;}
  label.code-label{
    font-family:'Baloo 2',sans-serif;
    font-weight:700;
    font-size:15px;
    color:var(--plum);
  }
  input#codeInput{
    width:100%;
    max-width:260px;
    text-align:center;
    letter-spacing:.5em;
    font-size:26px;
    font-weight:800;
    font-family:'Baloo 2',sans-serif;
    padding:14px 10px 14px 18px;
    border-radius:16px;
    border:3px solid var(--plum);
    background:#fff;
    color:var(--plum);
    outline:none;
  }
  input#codeInput:focus{border-color:var(--sky-deep);box-shadow:0 0 0 4px rgba(41,171,226,.2);}
  button#revealBtn{
    font-family:'Baloo 2',sans-serif;
    font-weight:700;
    font-size:17px;
    color:#fff;
    background:linear-gradient(135deg,var(--coral),#ff8a72);
    border:none;
    padding:14px 34px;
    border-radius:50px;
    cursor:pointer;
    box-shadow:0 10px 22px -8px rgba(255,111,89,.6);
    transition:transform .15s ease, box-shadow .15s ease;
  }
  button#revealBtn:hover{transform:translateY(-2px);box-shadow:0 14px 26px -8px rgba(255,111,89,.7);}
  button#revealBtn:active{transform:translateY(0);}
  .error-msg{
    color:var(--coral);
    font-weight:700;
    font-size:14px;
    text-align:center;
    min-height:18px;
  }

  .footer-note{
    text-align:center;
    font-size:12.5px;
    color:var(--plum-soft);
    margin-top:20px;
    font-weight:600;
    opacity:.8;
  }

  /* ---------- result view ---------- */
  #resultView{display:none;}
  .result-header{text-align:center;margin-bottom:18px;}
  .avatar-big{
    width:74px;height:74px;border-radius:50%;
    margin:0 auto 12px;
    display:flex;align-items:center;justify-content:center;
    font-family:'Baloo 2',sans-serif;font-weight:800;font-size:26px;
    color:#fff;
    box-shadow:0 10px 20px -8px rgba(46,37,64,.4);
  }
  .student-name{
    font-family:'Baloo 2',sans-serif;
    font-weight:800;
    font-size:22px;
    color:var(--plum);
  }
  .student-sub{
    font-size:13.5px;
    font-weight:700;
    color:var(--plum-soft);
    margin-top:2px;
  }

  .stamp{
    position:relative;
    margin:16px auto 20px;
    width:150px;height:150px;
    border-radius:50%;
    display:flex;flex-direction:column;align-items:center;justify-content:center;
    border:5px dashed;
    animation:stampIn .55s .2s cubic-bezier(.3,1.6,.4,1) both;
    background:#fff;
  }
  @keyframes stampIn{from{opacity:0;transform:scale(.4) rotate(-25deg);}to{opacity:1;transform:scale(1) rotate(-8deg);}}
  .stamp .num{font-family:'Baloo 2',sans-serif;font-weight:800;font-size:36px;line-height:1;}
  .stamp .lbl{font-family:'Baloo 2',sans-serif;font-weight:700;font-size:11px;letter-spacing:.06em;text-transform:uppercase;margin-top:4px;}
  .stamp .out-of{font-size:11px;font-weight:700;opacity:.7;}

  .bars{display:flex;flex-direction:column;gap:14px;margin:22px 0;}
  .bar-row .bar-label{
    display:flex;justify-content:space-between;
    font-family:'Baloo 2',sans-serif;
    font-weight:700;
    font-size:13.5px;
    margin-bottom:6px;
    color:var(--plum);
  }
  .bar-track{
    width:100%;height:14px;background:#EFE7F5;border-radius:20px;overflow:hidden;
  }
  .bar-fill{
    height:100%;border-radius:20px;
    width:0%;
    transition:width 1s cubic-bezier(.2,.9,.25,1);
  }

  .message-box{
    border-radius:18px;
    padding:18px 20px;
    text-align:center;
    font-weight:700;
    font-size:15px;
    line-height:1.5;
    margin:22px 0 8px;
  }
  .message-box .emoji{font-size:26px;display:block;margin-bottom:6px;}

  .again-btn{
    display:block;
    margin:18px auto 0;
    background:none;
    border:2px solid var(--plum);
    color:var(--plum);
    font-family:'Baloo 2',sans-serif;
    font-weight:700;
    font-size:14px;
    padding:10px 24px;
    border-radius:50px;
    cursor:pointer;
  }
  .again-btn:hover{background:var(--plum);color:#fff;}

  @media (max-width:420px){
    .passport{padding:26px 18px 24px;}
  }
</style>
</head>
<body>

<div class="trail" id="trail"></div>

<div class="stage">
  <div class="eyebrow">Yaz Okulu 2026</div>

  <div class="passport">
    <!-- ============ LANDING / CODE ENTRY ============ -->
    <div id="entryView">
      <div class="badge-row"><span class="plane">✈️</span></div>
      <h1 class="title">Bienvenue à l'annonce des résultats</h1>
      <div class="subtitle">Français A1 — Cours d'été</div>

      <div class="prof-card">
        <div class="prof-avatar">SE</div>
        <div class="prof-text">
          <div class="name">Prof : Seif Eddine</div>
          <div class="meta">Yaz Okulu 2026 · FRANÇAIS A1</div>
        </div>
      </div>

      <p class="lead">
        Bravo d'être arrivés jusqu'ici ! Vous avez travaillé tout l'été pour apprendre le français.
        Entrez votre code secret à 4 chiffres pour découvrir votre résultat. 🌟
      </p>

      <div class="code-form">
        <label class="code-label" for="codeInput">Code secret</label>
        <input type="text" id="codeInput" inputmode="numeric" maxlength="4" placeholder="••••" autocomplete="off">
        <div class="error-msg" id="errorMsg"></div>
        <button id="revealBtn">Voir mon résultat 🎉</button>
      </div>

      <div class="footer-note">Chaque élève a un code personnel — vos résultats sont privés.</div>
    </div>

    <!-- ============ RESULT VIEW ============ -->
    <div id="resultView">
      <div class="result-header">
        <div class="avatar-big" id="avatarBig"></div>
        <div class="student-name" id="studentName"></div>
        <div class="student-sub">Français A1 · Yaz Okulu 2026 · Prof. Seif Eddine</div>
      </div>

      <div class="stamp" id="stamp">
        <div class="num" id="stampNum"></div>
        <div class="out-of">/ 100</div>
        <div class="lbl" id="stampLbl"></div>
      </div>

      <div class="bars">
        <div class="bar-row">
          <div class="bar-label"><span>🗣️ Oral</span><span id="oralVal"></span></div>
          <div class="bar-track"><div class="bar-fill" id="oralBar" style="background:var(--sky);"></div></div>
        </div>
        <div class="bar-row">
          <div class="bar-label"><span>✍️ Écrit</span><span id="ecritVal"></span></div>
          <div class="bar-track"><div class="bar-fill" id="ecritBar" style="background:var(--coral);"></div></div>
        </div>
      </div>

      <div class="message-box" id="messageBox">
        <span class="emoji" id="messageEmoji"></span>
        <span id="messageText"></span>
      </div>

      <button class="again-btn" id="againBtn">← Vérifier un autre code</button>
    </div>
  </div>
</div>

<script>
const students = [
  {name:"ZEYNEP MİNA OĞUZ", code:"5486", oral:95, ecrit:89, total:92.0},
  {name:"MERT CANSIZ", code:"4333", oral:70, ecrit:81, total:75.5},
  {name:"CEREN KOÇER", code:"7183", oral:70, ecrit:89, total:79.5},
  {name:"CEREN GÜRÇAY", code:"0345", oral:70, ecrit:72, total:71.0},
  {name:"MUHAMMED TAYYİB USLU", code:"0914", oral:95, ecrit:85, total:90.0},
  {name:"ŞERİFE ŞEYMA DERE", code:"0757", oral:90, ecrit:88, total:89.0},
  {name:"ALMİRA AVŞAR", code:"8901", oral:75, ecrit:56, total:65.5},
  {name:"MÜBERRA KOCAKAYA", code:"0775", oral:80, ecrit:64, total:72.0},
  {name:"DURU KURT", code:"0761", oral:95, ecrit:92, total:93.5},
  {name:"ECEHAN MİRAY POLAT", code:"3849", oral:70, ecrit:76, total:73.0},
  {name:"BETÜL TANRIKUT", code:"1717", oral:70, ecrit:84, total:77.0},
  {name:"MACİD MACİT", code:"1896", oral:70, ecrit:60, total:65.0},
  {name:"ÇINAR NİZAMOĞLU", code:"7986", oral:95, ecrit:94, total:94.5},
  {name:"NURSENA CANER", code:"0374", oral:80, ecrit:47, total:63.5},
  {name:"SYED QAYYUM RAZA SHAH", code:"0274", oral:70, ecrit:96, total:83.0},
  {name:"BERRİN SOLAK", code:"0771", oral:70, ecrit:63, total:66.5},
  {name:"BADESU İZGİ", code:"0729", oral:90, ecrit:84, total:87.0},
  {name:"ELİF ZELAL ATA", code:"0774", oral:70, ecrit:75, total:72.5}
];

function tierFor(total){
  if(total >= 90) return {
    key:"excellent", color:"var(--gold)", ring:"#E6A817",
    label:"Excellent", emoji:"🏆",
    msg:"Félicitations ! Un résultat exceptionnel. Ton sérieux et ton travail tout l'été ont vraiment payé — continue comme ça, tu es sur la bonne voie !"
  };
  if(total >= 80) return {
    key:"tresbien", color:"var(--green)", ring:"#4CAF7D",
    label:"Très bien", emoji:"🌟",
    msg:"Très bien joué ! Tu as fait de très beaux progrès en français cet été. Encore un peu d'effort et l'excellence est à portée de main."
  };
  if(total >= 70) return {
    key:"bien", color:"var(--sky-deep)", ring:"#1C8FC2",
    label:"Bien", emoji:"👏",
    msg:"Bien joué, tu as de bonnes bases ! Continue à pratiquer l'oral et l'écrit, chaque jour tu deviens un peu plus à l'aise en français."
  };
  if(total >= 65) return {
    key:"assezbien", color:"var(--yellow)", ring:"#E0A93A",
    label:"Assez bien", emoji:"💪",
    msg:"C'est un bon début ! Tu as les capacités pour progresser encore. Un peu plus de pratique à l'oral et à l'écrit, et tes résultats vont vite s'améliorer."
  };
  return {
    key:"courage", color:"var(--coral)", ring:"#FF6F59",
    label:"Courage", emoji:"🌱",
    msg:"Ne baisse pas les bras ! Apprendre une langue prend du temps, et chaque leçon compte. Avec un peu plus de pratique, tu vas progresser rapidement — on croit en toi !"
  };
}

function initials(name){
  const parts = name.trim().split(/\s+/);
  const first = parts[0]?.[0] || "";
  const last = parts[parts.length-1]?.[0] || "";
  return (first+last).toUpperCase();
}

const entryView = document.getElementById('entryView');
const resultView = document.getElementById('resultView');
const codeInput = document.getElementById('codeInput');
const errorMsg = document.getElementById('errorMsg');
const revealBtn = document.getElementById('revealBtn');
const againBtn = document.getElementById('againBtn');

function showResult(student){
  const tier = tierFor(student.total);

  document.getElementById('avatarBig').textContent = initials(student.name);
  document.getElementById('avatarBig').style.background = `linear-gradient(135deg, ${tier.color}, var(--sky))`;
  document.getElementById('studentName').textContent = student.name;

  const stamp = document.getElementById('stamp');
  stamp.style.borderColor = tier.ring;
  document.getElementById('stampNum').textContent = student.total;
  document.getElementById('stampNum').style.color = tier.ring;
  document.getElementById('stampLbl').textContent = tier.label;
  document.getElementById('stampLbl').style.color = tier.ring;

  document.getElementById('oralVal').textContent = student.oral + " / 100";
  document.getElementById('ecritVal').textContent = student.ecrit + " / 100";

  const messageBox = document.getElementById('messageBox');
  messageBox.style.background = tier.color + "22";
  messageBox.style.color = "var(--plum)";
  document.getElementById('messageEmoji').textContent = tier.emoji;
  document.getElementById('messageText').textContent = tier.msg;

  entryView.style.display = "none";
  resultView.style.display = "block";

  requestAnimationFrame(()=>{
    setTimeout(()=>{
      document.getElementById('oralBar').style.width = student.oral + "%";
      document.getElementById('ecritBar').style.width = student.ecrit + "%";
    }, 80);
  });
}

function attemptReveal(){
  const code = codeInput.value.trim();
  if(code.length !== 4){
    errorMsg.textContent = "Merci d'entrer les 4 chiffres de ton code secret.";
    return;
  }
  const student = students.find(s => s.code === code);
  if(!student){
    errorMsg.textContent = "Code introuvable. Vérifie et réessaie.";
    codeInput.focus();
    return;
  }
  errorMsg.textContent = "";
  showResult(student);
}

revealBtn.addEventListener('click', attemptReveal);
codeInput.addEventListener('keydown', (e)=>{ if(e.key === 'Enter') attemptReveal(); });
codeInput.addEventListener('input', ()=>{
  codeInput.value = codeInput.value.replace(/[^0-9]/g,'').slice(0,4);
});

againBtn.addEventListener('click', ()=>{
  resultView.style.display = "none";
  entryView.style.display = "block";
  codeInput.value = "";
  errorMsg.textContent = "";
  codeInput.focus();
});

// decorative floating dots
(function(){
  const trail = document.getElementById('trail');
  const palette = ['#29ABE2','#FFC857','#FF6F59','#4CAF7D'];
  for(let i=0;i<14;i++){
    const d = document.createElement('div');
    d.className = 'dot';
    const size = 6 + Math.random()*14;
    d.style.width = size+'px';
    d.style.height = size+'px';
    d.style.left = Math.random()*100+'vw';
    d.style.top = Math.random()*100+'vh';
    d.style.background = palette[i % palette.length];
    d.style.filter = 'blur(1px)';
    trail.appendChild(d);
  }
})();
</script>

</body>
</html>
