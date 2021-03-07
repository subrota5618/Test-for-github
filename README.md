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
