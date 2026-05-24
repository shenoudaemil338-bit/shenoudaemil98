<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>القوانين الكشفية البحرية</title>

<style>
body{
    margin:0;
    font-family:Tahoma;
    background:#0b1f33;
    color:white;
}

header{
    background:linear-gradient(to right,#0077b6,#00b4d8);
    padding:30px;
    text-align:center;
}

header h1{
    font-size:40px;
}

section{
    padding:20px;
    margin:20px;
    background:#13293d;
    border-radius:15px;
    box-shadow:0 0 10px rgba(0,0,0,0.4);
}

h2{
    color:#4cc9f0;
}

ul li{
    margin:10px 0;
    font-size:18px;
}

button{
    background:#00b4d8;
    color:white;
    border:none;
    padding:10px 20px;
    border-radius:10px;
    cursor:pointer;
    font-size:18px;
    transition:0.3s;
}

button:hover{
    background:#0077b6;
    transform:scale(1.05);
}

.quiz{
    margin-top:20px;
}

.question{
    margin-bottom:20px;
}

footer{
    text-align:center;
    padding:20px;
    background:#001219;
    margin-top:30px;
}

.correct{
    color:lightgreen;
}

.wrong{
    color:red;
}
</style>
</head>

<body>

<header>
    <h1>⚓ القوانين الكشفية البحرية ⚓</h1>
    <p>موقع تعليمي عن قوانين ومهارات الكشافة البحرية</p>
</header>

<section>
    <h2>📜 قانون الكشاف</h2>

    <ul>
        <li>الكشاف صادق</li>
        <li>الكشاف أمين</li>
        <li>الكشاف نافع ويحب مساعدة غيره</li>
        <li>الكشاف صديق للجميع</li>
        <li>الكشاف مؤدب</li>
        <li>الكشاف رفيق بالحيوان</li>
        <li>الكشاف مطيع</li>
        <li>الكشاف بشوش</li>
        <li>الكشاف مقتصد</li>
        <li>الكشاف طاهر الفكر والقلب</li>
    </ul>
</section>

<section>
    <h2>🤝 الوعد الكشفي</h2>

    <p>
        أعد بشرفي أن أبذل جهدي في أن أقوم بواجبي نحو الله والوطن
        وأن أساعد الناس في جميع الظروف وأن أعمل بقانون الكشاف.
    </p>
</section>

<section>
    <h2>⚓ السلامة البحرية</h2>

    <ul>
        <li>ارتداء سترة النجاة</li>
        <li>عدم السباحة بدون إشراف</li>
        <li>معرفة إشارات الطوارئ</li>
        <li>الحفاظ على نظافة المياه</li>
    </ul>
</section>

<section class="quiz">
    <h2>📝 اختبار الكشافة البحرية</h2>

    <div class="question">
        <p>1- كم عدد بنود القانون الكشفي؟</p>

        <input type="radio" name="q1" value="صح"> 10<br>
        <input type="radio" name="q1" value="خطأ"> 5<br>
        <input type="radio" name="q1" value="خطأ"> 7<br>
    </div>

    <div class="question">
        <p>2- ماذا يجب ارتداؤه في البحر؟</p>

        <input type="radio" name="q2" value="صح"> سترة النجاة<br>
        <input type="radio" name="q2" value="خطأ"> قبعة فقط<br>
        <input type="radio" name="q2" value="خطأ"> حذاء رياضي<br>
    </div>

    <div class="question">
        <p>3- الكشاف يجب أن يكون؟</p>

        <input type="radio" name="q3" value="صح"> صادق<br>
        <input type="radio" name="q3" value="خطأ"> مهمل<br>
        <input type="radio" name="q3" value="خطأ"> كسول<br>
    </div>

    <button onclick="checkAnswers()">عرض النتيجة</button>

    <h3 id="result"></h3>
</section>

<footer>
    تم التصميم لخدمة الكشافة البحرية ⚓
</footer>

<script>
function checkAnswers(){

    let score = 0;

    let answers = document.querySelectorAll('input[value="صح"]:checked');

    score = answers.length;

    document.getElementById("result").innerHTML =
    "درجتك: " + score + " من 3";
}
</script>

</body>
</html>
