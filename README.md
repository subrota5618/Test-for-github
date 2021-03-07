$("#Log").click(function(){
var password1 = $("#pass1").val();
var password2 = $("#pass1").val();

if(password1!="" && password2!="")
{

if(password1==password2)
{

    alert("Login successfully");
}
 else{

alert("Sorry missmatch the password");
 }

}
else{

    alert("Enter your pasword");
}

});


<!DOCTYPE html>
<html lang="en">
     <style>
          #div{
               width: 280px;
               height:385px;
               background-color:darkcyan;
               border-radius: 22px;
               text-align: center;
          }
          .i{
     height:67px;
     width:250px;
     color: darkmagenta;
     background-color: cornflowerblue;
     font-size: 18px;

     border: 2px solid green;
     border-bottom:none;
}
.btn{

     height:55px;
     width:60px;
     background-color: chartreuse;
     color:blue;
     font-size:17px;
}

.btn:hover{
     transition-duration:1s;
     background-color:violet;
}
body{
     background-image: url(file:///F:/jj.png);
     background-color: coral;
}


     </style>
<head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <title>Calculator</title>
     <link rel="stylesheet" href="btn.css"/>
</head>
<body>
     <i style="font-size:25px; color: navy; font-family:ALGERIAN;">Nothing is impossible to a willing mind. Wish you all the best in everything you do.....</i>
     <br>   <br>  
     <div style="text-align: center;"> 
<div id="div"> 

     <marquee><i style="color:yellow;">Calculator.. Thanks for visit this link..</i></marquee>

     <br>  

  <form name="cal"> 
        <input type="text" name="display" class="i" placeholder="Directed by Diposh Chandra"/>
        <div>
             <input type="button" value="1" class="btn" onclick="cal.display.value+='1' ">
             <input type="button" value="2" class="btn" onclick="cal.display.value+='2' ">
             <input type="button" value="3" class="btn" onclick="cal.display.value+='3' ">
             <input type="button" value="+" class="btn" onclick="cal.display.value+='+' ">
        </div>
     
        <div>
          <input type="button" value="6" class="btn" onclick="cal.display.value+='6'">
          <input type="button" value="5" class="btn" onclick="cal.display.value+='5'">
          <input type="button" value="4" class="btn" onclick="cal.display.value+='4'" >
          <input type="button" value="-" class="btn" onclick="cal.display.value+='-'">
     </div>

     <div>
          <input type="button" value="9" class="btn" onclick="cal.display.value+='9'">
          <input type="button" value="8" class="btn" onclick="cal.display.value+='8'">
          <input type="button" value="7" class="btn" onclick="cal.display.value+='7'">
          <input type="button" value="X" class="btn" onclick="cal.display.value+='*'">
     </div>

     <div>
          <input type="button" value="0" class="btn" onclick="cal.display.value+='0'">
          <input type="button" value="^" class="btn" onclick="cal.display.value+= '^'">
          <input type="button" value="%" class="btn" onclick="cal.display.value+='%'">
          <input type="button" value="/" class="btn"  onclick="cal.display.value+='/'">
     </div>

     <div>
          <input type="button" value="." class="btn"  onclick="cal.display.value+='.'">
          <input type="button" value="C" class="btn"  style="background-color: darkblue; color: chartreuse;" onclick="cal.display.value=''" id="del">
          <input type="button" value="DEL" class="btn"  style="background-color: darkblue; color: coral;" onclick="cal.display.value ='' " id="del">
          <input type="button" value="=" class="btn" style="background-color: darkblue; color: yellow;" onclick="cal.display.value  =eval(cal.display.value)">
     </div>

</form>


</div>
</div>
<script src="calcu.js"></script>
</body>
</html>

var cal = $("#result") . val();

function insertNumber(number){

    var existingNumbers = cal ;


    cal(existingNumbers+number);

}
function clearNumber()
{

    cal ('');
}

function calculateNumber(){
  var result = eval(  $("#result").val());
  cal (result)

}
function deleteNumbers(){


    var pre=   $("#result").val();

    if(pre!='')
    {

    
    $("#result").val(pre.slice(0,-9));

    }
}


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <canvas height="233" width="356" id="demo"></canvas>
<br><br>

<script>
     var canvas = document.getElementById("demo");
                var context =  canvas.getContext("2d");
context.fillStyle="green";
                context.fillRect(12,13,367,233);

                     var centerX  =  canvas.width/2;
                     var centerY = canvas.height/2;

                     context.beginPath();

                      context.arc(centerX,centerY,67,0,2*Math.PI, false);
                         context.fillStyle="red";
                          context.fill();
</script>

</body>
</html>
