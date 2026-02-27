<!DOCTYPE html>
<html lang="sw">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>KAMUSI YA KIZIMAMOTO PRO</title>

<style>
body{
    margin:0;
    font-family: Arial, Helvetica, sans-serif;
    background:#0f172a;
    color:white;
}

header{
    background:linear-gradient(90deg,#b91c1c,#7f1d1d);
    padding:20px;
    text-align:center;
    font-size:28px;
    font-weight:bold;
    letter-spacing:2px;
}

.search-box{
    text-align:center;
    margin:20px;
}

input{
    width:80%;
    padding:12px;
    font-size:16px;
    border-radius:8px;
    border:none;
}

.container{
    padding:20px;
    display:grid;
    grid-template-columns: repeat(auto-fit,minmax(300px,1fr));
    gap:20px;
}

.card{
    background:#1e293b;
    padding:20px;
    border-radius:12px;
    box-shadow:0 0 10px rgba(0,0,0,0.6);
    transition:0.3s;
}

.card:hover{
    transform:scale(1.03);
    background:#334155;
}

h2{
    color:#f87171;
}

footer{
    text-align:center;
    padding:20px;
    background:#111827;
    margin-top:30px;
}
</style>
</head>

<body>

<header>
🔥 KAMUSI KUBWA YA MANENO YA KITAALAMU YA ZIMAMOTO 🔥
</header>

<div class="search-box">
<input type="text" id="searchInput" placeholder="Andika neno la kizimamoto kutafuta...">
</div>

<div class="container" id="wordContainer">

<div class="card">
<h2>Fire Tetrahedron</h2>
<p>Nadharia inayoelezea kuwa moto unahitaji vitu vinne: Joto (Heat), Mafuta (Fuel), Oksijeni (Oxygen) na Mmenyuko wa Kikemikali (Chemical Chain Reaction). Kuondoa kipengele kimoja huzima moto.</p>
</div>

<div class="card">
<h2>Flashover</h2>
<p>Hatua ya ghafla ambapo gesi zote zinazowaka ndani ya chumba zinawaka kwa wakati mmoja kutokana na joto kali kufikia kiwango cha kuwaka.</p>
</div>

<div class="card">
<h2>Backdraft</h2>
<p>Mlipuko unaotokea pale oksijeni inapoingia ghafla katika eneo lenye moto uliokuwa umefungiwa bila hewa ya kutosha.</p>
</div>

<div class="card">
<h2>SCBA (Self Contained Breathing Apparatus)</h2>
<p>Kifaa cha kupumulia hewa safi kinachovaliwa na askari wa zimamoto wakati wa operesheni katika mazingira yenye moshi au gesi hatari.</p>
</div>

<div class="card">
<h2>Fire Load</h2>
<p>Kiasi cha vitu vinavyoweza kuwaka ndani ya eneo fulani ambacho kinaweza kuongeza ukubwa wa moto.</p>
</div>

<div class="card">
<h2>Compartment Fire</h2>
<p>Moto unaotokea ndani ya chumba kilichofungwa au jengo lenye mipaka maalumu ya kuta.</p>
</div>

<div class="card">
<h2>Ventilation</h2>
<p>Utaratibu wa kuingiza au kutoa hewa ili kupunguza joto, moshi na gesi hatari wakati wa uokoaji.</p>
</div>

<div class="card">
<h2>Hydrant</h2>
<p>Kifaa cha kudumu kinachounganishwa na mfumo wa maji kwa ajili ya kujaza maji kwenye gari la zimamoto.</p>
</div>

<div class="card">
<h2>Fire Suppression System</h2>
<p>Mfumo wa kiotomatiki wa kuzima moto kama sprinkler system au mfumo wa gesi ya CO₂.</p>
</div>

<div class="card">
<h2>Incident Command System (ICS)</h2>
<p>Mfumo wa uongozi unaotumika kusimamia matukio ya dharura kwa mpangilio wa kitaalamu na mgawanyo wa majukumu.</p>
</div>

<div class="card">
<h2>Thermal Layering</h2>
<p>Mgawanyiko wa joto ndani ya chumba ambapo hewa ya moto hukusanyika juu na baridi chini.</p>
</div>

<div class="card">
<h2>Fire Behavior</h2>
<p>Tabia ya moto kuenea, kubadilika na kuathiri mazingira kulingana na hewa, joto na aina ya mafuta yanayowaka.</p>
</div>

</div>

<footer>
© 2026 KAMUSI YA ZIMAMOTO PRO | Mfumo wa Mafunzo na Marejeo ya Kitaalamu
</footer>

<script>
const searchInput = document.getElementById("searchInput");
const cards = document.querySelectorAll(".card");

searchInput.addEventListener("keyup", function(){
    let filter = searchInput.value.toLowerCase();
    cards.forEach(card => {
        let text = card.innerText.toLowerCase();
        if(text.includes(filter)){
            card.style.display="block";
        } else {
            card.style.display="none";
        }
    });
});
</script>

</body>
</html>
