# gk-test-study-kunji
Education Learning Center 


<!DOCTYPE html>
<html lang="hi">
<head>
<meta charset="UTF-8">
<title>STUDY KUNJI - GK Online Test</title>
<style>
body{font-family:Arial;background:#f4f6f8;padding:20px}
.box{max-width:700px;margin:auto;background:#fff;padding:20px;border-radius:8px}
h1{text-align:center;color:#2c3e50}
.question{margin:15px 0}
button{padding:10px 20px;font-size:16px;background:#27ae60;color:#fff;border:none;border-radius:5px}
</style>
</head>

<body>
<div class="box">
<h1>STUDY KUNJI<br>GK Online Test</h1>

<form id="quizForm">

<div class="question">
<b>1. भारत की राजधानी क्या है?</b><br>
<input type="radio" name="q1" value="0"> मुंबई<br>
<input type="radio" name="q1" value="1"> नई दिल्ली<br>
<input type="radio" name="q1" value="0"> कोलकाता<br>
<input type="radio" name="q1" value="0"> चेन्नई
</div>

<div class="question">
<b>2. भारत के प्रथम राष्ट्रपति कौन थे?</b><br>
<input type="radio" name="q2" value="1"> डॉ. राजेंद्र प्रसाद<br>
<input type="radio" name="q2" value="0"> नेहरू<br>
<input type="radio" name="q2" value="0"> गांधी<br>
<input type="radio" name="q2" value="0"> पटेल
</div>

<div class="question">
<b>3. ताजमहल कहाँ है?</b><br>
<input type="radio" name="q3" value="1"> आगरा<br>
<input type="radio" name="q3" value="0"> दिल्ली<br>
<input type="radio" name="q3" value="0"> जयपुर<br>
<input type="radio" name="q3" value="0"> लखनऊ
</div>

<div class="question">
<b>4. राष्ट्रीय पशु?</b><br>
<input type="radio" name="q4" value="1"> बाघ<br>
<input type="radio" name="q4" value="0"> शेर<br>
<input type="radio" name="q4" value="0"> हाथी<br>
<input type="radio" name="q4" value="0"> घोड़ा
</div>

<div class="question">
<b>5. सूर्य कहाँ से उगता है?</b><br>
<input type="radio" name="q5" value="1"> पूर्व<br>
<input type="radio" name="q5" value="0"> पश्चिम<br>
<input type="radio" name="q5" value="0"> उत्तर<br>
<input type="radio" name="q5" value="0"> दक्षिण
</div>

<button type="button" onclick="result()">Submit Test</button>
</form>

<h2 id="score"></h2>
</div>

<script>
function result(){
let total=5,score=0;
for(let i=1;i<=5;i++){
let q=document.querySelector('input[name="q'+i+'"]:checked');
if(q){score+=parseInt(q.value);}
}
document.getElementById("score").innerHTML=
"आपका Score: "+score+" / "+total;
}
</script>
</body>
</html>
