
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=Edge">
  <meta name="viewport" content="width=device-width, initial-scale=1">

<body style="background-color:deeppink;">

Created By-Suzal

 
   <body style="background-color:light deeppink;">




<!DOCTYPE html>
<html>
<head>
 <title></title>
 <!-- Latest compiled and minified CSS -->
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.2.1/css/bootstrap.min.css">

<body style="background-color:deeppink;"


<style >
 body{
 
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  width: 100%;
  height: 100vh;
  position: relative;
 }
 header{
  width: 100%;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
 }
</style>
</head>
<body>

<header >
 
<div class="card w-50 m-auto text-center ">
  <div class="card-header bg-danger text-white">LOVE CALCULATOR</div>
  <div class="card-body">
   <form class="form-inline w-75 m-auto">
    <div class="form-group">
     <input type="text" name="" class="form-control text-center" placeholder="Your Name" id="name" >
    </div>
    <div class="pl-4 pr-4">
     <span> + </span>
    </div>
    <div class="form-group">
     <input type="text" name="" class="form-control text-center" placeholder=" Crush Name" id="lname">
    </div>
   </form> <br>
    <div class="w-70 m-auto">
     <button  class="btn btn-success w-50" onclick="checkloveper()"> click </button>
    </div>
    <br>
    <div>
     <input type="text" name="" placeholder="LOVE PERCENTAGE" class="form-control text-center w-25 m-auto" id="lovevalue">
    </div>
  </div> 
  <div class="card-footer ">Best of luck</div>
</div>

</header>

<script>
 function checkloveper(){

  var name = document.getElementById('name').value;
  var lname = document.getElementById('lname').value;

  if(name == ""){
   alert('Please enter your name');
  }else if (name.length <=2 ) {
   alert('Min lenght is 3')
  }else if(!isNaN(name)){
   alert('Numbers are not allowed');
  }

  else if(lname == ""){
   alert('Please enter your love name');
  }else if (lname.length <=2 ) {
   alert('Min lenght is 3')
  }else if(!isNaN(lname)){
   alert('Numbers are not allowed');
  }
  else{
  var lovdata = Math.random() * 100;
  lovdata = Math.floor(lovdata);
  document.getElementById('lovevalue').value = lovdata + "%"; 
  }
  
 }
</script>
</body>

</html>
