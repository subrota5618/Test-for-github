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


<br>
 <!DOCTYPE html>
<html lang="en">
<head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <title>Bootstrap 4</title>

     <link rel="stylesheet" href="/css/bootstrap.min.css">
     <link rel="stylesheet" href="k.css">
</head>
<body>

     //Link are here//
     <div  class="justify-content-center bg-secondary"> 
         

          <ul class="nav justify-content-center">
               <img src=" file:///F:/kk.jpg " class="sm-4 md-4 fluid rounded-circle" style="height: 38px; width: 38px;"/>  
          <li class="nav-item"> <a href="file:///C:/Users/user/Desktop/b%20test/s.html#" target="blank" class=" nav-link">Home</a> </li>
<li class="nav-item"> <a href="file:///C:/Users/user/Desktop/b%20test/form.html" target="blank" class=" nav-link">Comment</a></li>
<li class="nav-item"><a href="file:///C:/Users/user/Desktop/b%20test/n.html" target="blank" class="nav-link">Website</a></li>
<li class="nav-item"> <a href="file:///C:/Users/user/Desktop/b%20test/n.html" target="blank" class="nav-link">Privacy</a> </li>

</ul>
</div>
//div image//
     <div style="background-image: url(file:///F:/kk.jpg);"> 
        <br>
        <h2 class="text-primary text-md-center">Diposh Chandra Sharkar</h2>
        <br>  <br>  <br><br>  <br>
       
     <div class="">

     <ul class="pagination justify-content-center" >
        

<li class="page-link">
               <a href="https://youtube.com/" target="blank">
                    <img src="file:///D:/Users/user/Pictures/you.PNG" class="justify-content-center page-link bg-primary" />
               </a>
</li>

<li class="page-link">
     <a href="https://accounts.google.com/b/0/AddMailService" target="blank">
          <img src="file:///D:/Users/user/Pictures/gg.PNG " class="justify-content-center page-link bg-info"/>
     </a>
</li>
               </ul>
</div>

     
          <br><br><br><br>
          <p class="text-info text-md-center">
               Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quas dolore sapiente pariatur culpa, eveniet beatae aliquam nostrum voluptas voluptatum officia, nulla illo et veniam numquam deleniti dolorem harum nihil? Corporis recusandae, impedit totam, fugit omnis ducimus, nisi velit nobis architecto vitae sequi maxime harum?
          </p>
          <i class="text-success">Lorem ipsum dolor sit amet consectetur adipisicing elit. Reiciendis ratione molestias ullam blanditiis repellendus fugit quam eligendi inventore ducimus quis! Repellat, non consectetur? Ipsa, assumenda omnis culpa nulla nam iure, deserunt distinctio velit veritatis fuga praesentium animi non recusandae harum mollitia itaque totam consequuntur sint asperiores esse! Praesentium architecto voluptate molestias ullam rerum, voluptates tempore illo.</i>
     </div>
     <br><br>
     <div class="container bg-info text-white">
          <img src=" file:///F:/kk.jpg " class="sm-4 md-4 fluid rounded-circle" style="height: 38px; width: 38px;"/>  
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Quasi, qui. Dolor blanditiis est quae id eligendi sapiente neque ducimus totam quasi quia, quod voluptates consequuntur rerum saepe similique asperiores. Quia dolorum assumenda culpa soluta cumque corrupti dolores dignissimos! Voluptatum similique fuga porro quos, perferendis optio inventore quidem esse necessitatibus odit consectetur placeat dolor qui maiores!
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio, suscipit eligendi ad recusandae, omnis tempore ea rerum nobis, facilis accusantium dolor quas voluptas nisi possimus ipsa? Blanditiis incidunt quia aspernatur repellendus laboriosam? Provident iure accusantium, veniam debitis quam rem voluptatum delectus facere est. Possimus doloremque ipsam iusto similique minima tempora vitae quae inventore magni autem. Eum repellat expedita vero sit ipsa labore totam quae quod! Numquam, distinctio! Animi nihil laudantium modi quidem debitis aspernatur quis? Voluptates, qui architecto!
   
</div>
//Button are here//
<br><br>

<p class="bg-warning text-info"> 

Lorem ipsum dolor sit, amet consectetur adipisicing elit. Iusto labore esse necessitatibus placeat, expedita et odio, veniam illum ipsum soluta, officiis vero maiores. Magni quam molestias iure eius sapiente inventore.
Lorem ipsum dolor sit amet consectetur adipisicing elit. Sapiente, facere modi eos eius cum assumenda reiciendis quod illo sed ut quidem aperiam ad?
</p>
<br><br>

<button class="btn-primary">click me</button>
<br><br>

//image are hre//

<br><br>
<input type="button" value="click me" onclick="alert('hello my friend')" class="btn-outline-primary">



<br><br>
<div class="container bg-info text-warning">
     <i class="fas fa-facebook"></i>
  
     
<i class="fas fa-hand">

     <img src="file:///F:/time.png" class="fluid rounded-circle  " style="height: 28px; width:29px;">

 
     <br>
 
 Lorem ipsum dolor sit amet consectetur adipisicing elit. Quaerat, sint deleniti qui suscipit possimus aliquam pariatur rem quas expedita. Magnam, eos! Ad unde aperiam perspiciatis id? Qui quis nulla cum et accusamus unde asperiores ullam aut, quibusdam tenetur magni consequatur atque, in amet aperiam, doloremque cumque nostrum adipisci? Quos odit, dolor ratione labore facere voluptatibus magnam est harum corrupti inventore, unde itaque exercitationem, corporis voluptas tempora in?
</div>


<div class="collapse" id="demo">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Expedita architecto ducimus eos et, perferendis, nesciunt vero, qui atque tempore corporis quae accusantium pariatur molestias saepe dicta culpa? Dignissimos atque in, quia eum aliquid alias nemo! Blanditiis veniam veritatis debitis hic natus accusantium totam, numquam </div>
<br><br>
//From is here//
<div class="bg-success text-secondary">

<form action="mail-to:subrotachandrasarker20@gmail.com" method="post" class="w-50 m-auto" id="p">
     <br>
<h2 class="text-center">comment me</h2>
     <br>

Full Name:<input type="text" placeholder="Enter your name" class="form-control"/>

<br><br>
Textfield:
<textarea style="height:144px;" class="form-control">Type your text here..</textarea>
<br><br>
Email:<input type="email" value="Email" class="form-control"/>
<br><br>
<input type="submit" value="submit" class="btn-outline-info"/>
|
<input type="reset" value="Reset" class="btn-outline-warning"/>
</form>
</div>
//pagination is here//
<br><br><br>
<div class="container" style="background-color: rebeccapurple;">

     <br><br>
<div class="container bg-blcak justify-content-center">

     <div class="bg-info text-md-center">About me</div>

     <div class="bg-warning text-md-center " id="i">This website</div>

     <div class="bg-blcak text-md-center" id="i"> Developer</div>
     
     <div class="bg-primary text-md-center">Contact me</div>
     <br> <br>

<ul class="pagination justify-content-center">
     <li class="page-item "><a href="file:///C:/Users/user/Desktop/b%20test/about%20me.html" target="blank" class="page-link bg-secondary">1</a></li>
     
     <li class="page-item"><a target="blank" href="file:///C:/Users/user/Desktop/b%20test/h.html" class="page-link  bg-primary">2</a></li>
     <li class="page-item "><a target="blank" href="file:///C:/Users/user/Desktop/b%20test/n.html" class="page-link bg-secondary">3</a></li>
     
     <li class="page-item "><a target="blank" href="  file:///C:/Users/user/Desktop/b%20test/form.html " class="page-link bg-success" >4</a></li>
</ul>
</div>
</div>
//pagination End//


<div class="bg-warning tex-info">
     <p class="border border-danger">Lorem ipsum dolor sit amet consectetur adipisicing elit. Nemo nesciunt inventore excepturi voluptates illum eligendi commodi veniam quod, sequi voluptate aspernatur repellat.</p>
<p class="border ">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Voluptates beatae minima odit libero nulla possimus modi perferendis laborum quam. Ullam, perferendis.</p>
</div>
//Border end//

<div class="border ml-6 pr-34 media border-warning bg-success">
   
          <img src="file:///F:/kk.jpg" class="thumbanail fluid  rounded-circle mr-4 align-self-center" style="height:46px; width:37px;">
         <div class="media-body pr-12 ">
          <p class="text-warning">
     Sint facere repudiandae illo officiis ad tempora, nobis itaque quidem asperiores, magni labore, iste numquam fugit corporis eveniet velit. Delectus dolor numquam totam nihil nobis ut, similique sint cupiditate temporibus iste culpa natus maiores laboriosam, deleniti explicabo.
         </p>
         </div>
</div>

//end border//
<table class="table">

<tr>
     <td> 
     <div class="div2 bg-5" id="scale" style="background-color: darkslategrey;">
     <img src="file:///F:/kk.jpg" class="thumbanail fluid  rounded-circle mr-4 justify-content-center" style="height:46px; width:37px;">
     <br>
     <p style="color: blueviolet;"> 
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Aspernatur ex sapiente nisi, maxime rem saepe distinctio inventore ipsa.</p>
</div>
</td>

<td> 
<div class="div2" id="scale" style="background-color: darkslategrey;">
     <img src="file:///F:/kk.jpg" class="thumbanail fluid  rounded-circle mr-4 justify-content-center" style="height:46px; width:37px;">
     <br>
     <p style="color: blueviolet;"> 
    Lorem, ipsum dolor sit amet consectetur adipisicing elit. Illo ut necessitatibus voluptas fugiat nobis, laudantium quia sit ad.  </p>
</div>
</td>
<td> 
     <div class="div2" id="scale" style="background-color: darkslategrey;">
     <img src="file:///F:/kk.jpg" class="thumbanail fluid  rounded-circle mr-4 justify-content-center" style="height:46px; width:37px;">
     <br>
     <p style="color: blueviolet;"> 
  Lorem ipsum dolor sit amet consectetur adipisicing elit. Eaque beatae, voluptatibus ad nam labore suscipit rerum repellendus iste! </p>
</div>
</td>
<td> 
<div class="div2" id="scale" style="background-color: darkslategrey;">
     <img src="file:///F:/kk.jpg" class="thumbanail fluid  rounded-circle mr-4 justify-content-center" style="height:46px; width:37px;">
     <br>
     <p style="color: blueviolet;"> 
  Lorem ipsum, dolor sit amet consectetur adipisicing elit. Aperiam commodi culpa porro maiores praesentium laborum fugit non qui!  </p>
</div>
</td>

</tr>
</table>
//End hover//
<br>
//nav is here//
<ul class="nav nav-pills">
     <li class="nav-item"><a data-toggle="pill" href="#edu" class="nav-link">Education</a></li>
     <li class="nav-item"><a data-toggle="pill" href="#skill" class="nav-link" >Skill</a></li>
     <li class="nav-item"><a data-toggle="pill" href="#hobby" class="nav-link">Hobby</a></li>

</ul>

<div class="tab-content">

     <div id="edu" class="tab-pane fade">
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Velit impedit nam dolorum hic similique dolor! Molestiae sapiente ullam id error. Sint sunt maxime dicta voluptates? Quo quos accusantium vero temporibus odit unde minima.</p>
     </div>
     <div  id="skill" class="tab-pane fade">
          <p style="color: cornflowerblue;"> 22.Lorem ipsum dolor sit amet consectetur adipisicing elit. Velit impedit nam dolorum hic similique dolor! Molestiae sapiente ullam id error. Sint sunt maxime dicta voluptates? Quo quos accusantium vero temporibus odit unde minima.</p>
     </div>

     <div  id="hobby" class="tab-pane fade">
          <p style="color: blue;">66.Lorem ipsum dolor sit amet consectetur adipisicing elit. Velit impedit nam dolorum hic similique dolor! Molestiae sapiente ullam id error. Sint sunt maxime dicta voluptates? Quo quos accusantium vero temporibus odit unde minima.</p>
     </div>
</div>
//close button//

<div class="col-sm-4 col-lg-6">
     <p class="bg-dark text-warning">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Deleniti magni cumque modi?
     </p>
     <br></br>
     //base//

<div class="alert alert-dismissable bg-success">

<button class="close" data-dismiss="alert">&times;</button>
    Are you like this webpage to gather the experience.
    <a href="#">Visit me.</a>
</div>
//table strat//
<br><br>
<table class="table table-bordered bg-success table-hover text-info table-warninig">

     <tr class="bg-secondary">
          <th>Name</th>
          <th>Class</th>
          <th>G.P.A</th>
     </tr>
     <tr>
          <td>Subrota Chandra Sarker</td>
          <td>J.S.C</td>
          <td>3.85</td>
     </tr>
     
     <tr>
          <td rowspan="2">Subrota Chandra Sarker</td>
          <td>S.S.C</td>
          <td rowspan="2">4.06</td>
     </tr>
     <tr>
          <td>Science</td>
     </tr>
     <tr>
          <td rowspan="2">Subrota Chandra Sarker</td>
          <td>H.S.C</td>
          <td rowspan="2">3.67</td>
     </tr>
     <tr>
          <td>Science</td>
     </tr>
</table>
<br><br>
<br><br>
<table class="table table-bordered table-hover text-center text-info table-danger">

     <tr class="bg-secondary">
          <th colspan="4">Name</th>
          <th>Class</th>
          <th >G.P.A</th>
          <th colspan="4">Name</th>
          <th>Class</th>
          <th >G.P.A</th>

     </tr>
     <tr>
          <td colspan="4">Subrota </td>
          <td>J.S.C</td>
          <td>3.85</td>
          <td colspan="4">Subrota </td>
          <td>J.S.C</td>
          <td>3.85</td>
     </tr>
     
     <tr>
          <td colspan="4">Subrota </td>
          <td>S.S.C</td>
          <td>4.06</td>
          <td colspan="4">Subrota </td>
          <td>J.S.C</td>
          <td>3.85</td>
     </tr>
   
     <tr>
          <td colspan="4">Subrota </td>
          <td>P.S.C</td>
          <td>4.58</td>
          <td colspan="4">Subrota </td>
          <td>J.S.C</td>
          <td>3.85</td>
     </tr>
     <tr>
          <td  colspan="4">Subrota </td>
          <td>H.S.C</td>
          <td>3.67</td>
          <td colspan="4">Subrota </td>
          <td>J.S.C</td>
          <td>3.85</td>
     </tr>
</table>
//table end//
<br>
//button//
 
<button onclick="msg()" style="background-color: aqua;">Delete</button>

<script>
     function msg()
     {

var v = confirm("are sure to delete this file?");

if(v==true)
{
     alert("Delete");
}
else{
     alert("Cancel");
}

     }
</script>
<script src="s.js"></script>
</body>
</html>


<br>
PHP code start from here......................
<br>
<?php

//unshift array//
 $array = array('a' =>'Hindi' , 'b' =>'Spanis' , 'c' =>'Telugu');

array_unshift($array, 'Bangla','English');

echo "<pre>";
print_r($array);
echo  "</pre>"
?>
<br>
<?php

//Incremenet and Decremenet//

echo"45 is the variable";
echo "<br>";
$b=45;

$b--;
echo $b;

?>

<br>
<?php

//Incremenet and Decremenet//

echo"45 is the variable";
echo "<br>";
$b=45;

$b++;
echo $b;

?>

<br>
<?php

//Incremenet and Decremenet//

echo"45 is the variable";
echo "<br>";
$b=45;

--$b;
echo $b;

?>

<br>
<?php

//Incremenet and Decremenet//

echo"45 is the variable";
echo "<br>";
$b=45;

++$b;
echo $b;

?>
<br>
<?php

$a=34;
$a++;
echo  $a;

?><?php
/*
$a=34;
++$a;
echo ++$a;

echo --$a;
*/
/*
$a=array(12,56,67,78);
foreach($a as $c)
{
echo $c."<br>";
}*/

$a=array (59,56,"heloo","Key");
foreach($a as $c)
{

     echo"$c <br>";
}
?>
<br>
<?php
$city=("gh","jh","ghg","fhfg");

for ($ of city) { 
     echo "$city <br>";
}
?>

<?php
//while  Loop//
$a=5;
while($a<34)
{
print("Hello I am while Loop. <br>" ); $a++;
}

?>
<br>
<?php
//for Loop without var//

for($a<56; $a=0; $a++)
{
     print("Hello I am for Loop use me without var");
}
?>
<br>
<?php
//do while loop//
$a=1;

do{
     print("Hello I am do while Loop<br>"); $a++;
}while($a<23);

?>
<br>
<?php
$c=4;
do{
     print("Hello just check it <br>"); $c++;
}
while($c<45);

?>
<?php
/*
* Change the value of $password if you have set a password on the root userid
* Change NULL to port number to use DBMS other than the default using port 3306
*
*/
$user = 'root';
$password = ''; //To be completed if you have set a password to root
$database = 'jeni'; //To be completed to connect to a database. The database must exist.
$port = NULL; //Default must be NULL to use default port
$mysqli = new mysqli('127.0.0.1', $user, $password, $database, $port);

if ($mysqli->connect_error) {
    die('Connect Error (' . $mysqli->connect_errno . ') '
            . $mysqli->connect_error);
}
echo '<p>Connection OK '. $mysqli->host_info.'</p>';
echo '<p>Server '.$mysqli->server_info.'</p>';
echo '<p>Initial charset: '.$mysqli->character_set_name().'</p>';

$mysqli->close();
?>
PHP end here........................


</body>
</html>
