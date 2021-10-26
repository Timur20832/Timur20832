var arr2 = '';
var arr3 = '';
var arr4 = '';
var arr5 = '';
var arr6 = '';
document.getElementById('param-1').oninput = function () {
    // ползунок - длина массива
 document.getElementById('password-length').innerHTML = this.value;
}
var 
result,
b = document.getElementByName('name1').value,
y = document.getElementByName('name2').value,
z = document.getElementByName('name3').value,
k = document.getElementByName('name4').value ,
c = document.getElementByName('name5').value,
m =document.getElementByName('name6').value ;

    document.getElementByName('param-2').onclick = generate();
    document.getElementById('out').result = '';
    console.log(result);

function generate() {
    result = b+y+z+k+c+m;
    alert(result);
}
function compareRandom(a, b) {
    return Math.random() - 0.5;
}

function randomInteger(min, max) {
    var rand = min - 0.5 + Math.random() * (max - min + 1)
    rand = Math.round(rand);
    return rand;
}
//html
<!doctype html>
<html>
    <head>
      <meta charset="utf-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>Bootstrap сайт</title>
      <link rel="stylesheet" href="css/bootstrap.css">
      <link rel="stylesheet" href="css/font-awesome.min.css">
      <link rel="stylesheet" href="css/main.css">
    </head>
<body>
    <div class="navbar navbar-inverse navbar-fixed-top">
      <div class="container">
        <div class="navbar-header">
          <a class="navbar-brand" href="#">Наш сайт<i class="fa fa-unlock-alt"></i></a>
          </div>
            <div class="navbar-collapse collapse">
            <ul class="nav navbar-nav navbar-right">
            <li class="active"><a href="./index.html">Домой</a></li>
          </ul>
        </div>
      </div>
    </div>
      <div id="background">
        <div class="container">
            <form action="#" method="#" id="form">
              <div>
                <div class="form-group">
                  <label for="param-1">Длина строки (<span id="password-length">10</span>)</label>
                  <input type="range" class="form-control" id="param-1" value="10" max="50">
              </div>
            <label>
              Ваша дата рождения?
              <input type="text" name="name1" >
          </label>
    </div>
    <div>
  <label>
  Как зовут вашего лучшего друга?
  <input type="text" name="name2" >
  </label>
  </div>
    <div>
    <label>
    Какая ваша любимая книга?
    <input type="text" name="name3" >
    </label>
    </div>
      <div>
      <label>
      Ваш любимый цвет?
      <input type="text" name="name4" >
      </label>
      </div>
          <div>
          <label>
          Последние три цифры вашего номера телефона:
          <input type="text" name="name5" >
          </label>
          </div>
    <button type="button" class="shiza" name ="param-2" onclick = "generate()" >Отправить</button>
          </div>
        </div>
</div>
<div class="row">
  <div class="col-lg-12">
      <div id="out">
        
      </div>
  </div>
</div>
</div>
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.0/jquery.min.js"></script>
  <script src="js/bootstrap.min.js"></script>
  <script src="js/kod.js"></script>
</body>
</html>
