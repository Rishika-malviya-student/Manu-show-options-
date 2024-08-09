# Manu-show-options-
This is a simple land landing page for the study purpose and it is a very simple webpage to click for media options like instagram ,Facebook ,Twitter ,WhatsApp.
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Share Button</title>
<link rel="stylesheet" href="style.css">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta2/css/all.min.css" integrity="sha512-YWzhKL2whUzgiheMoBFwW8CKV4qpHQAEuvilg9FAn5VJUDwKZZxkJNuGM4XkWuk94WCrrwslk8yWNGmY1EduTA==" crossorigin="anonymous" referrerpolicy="no-referrer" />
<style> 
HTML CSS Result Skip Results Iframe
*{
margin: 0;
padding: 0;
box-sizing: border-box;
}
body{
display: flex;
justify-content: center;
align-items: center;
height: 100vh;
}
.container{
width: 40px;
height: 40px;
position: relative;
}
.container input{
position: absolute;
width: 100%;
height: 100%;
appearance: none;
-webkit-appearance: none;
cursor: pointer;
}
.container input::before{
content: "\f1e0";
position: absolute;
font-family: 'Font Awesome 6 Free';
font-weight: 700;
font-size: 1.5rem;
top: 0;
left: 0;
width: 100%;
height: 100%;
background: #9733EE;
color: white;
border-radius: 50%;
display: flex;
justify-content: center;
align-items: center;
}
.container input:checked::before{
content: "\f00d";
font-size: 2rem;
}
.container input::after{
content: "";
position: absolute;
top: -35%;
left: -35%;
width: 120%;
height: 120%;
z-index: -10;
border: 10px solid #9733EE;
box-shadow: 0 0 30px #9733ee4f;
border-radius: 0%;
transform: scale(.5);
transition: all .4s;
}
.container input:checked::after{
transform: scale(1.5);
border-radius: 50%;
}
.links{
position: absolute;
z-index: -10;
}
.container input:checked ~ .links{
transition: all 4s;
z-index: 50;
}
.links a{
position: absolute;
width: 40px;
height: 40px;
text-decoration: none;
display: flex;
justify-content: center;
align-items: center;
background: rgba(0, 0, 0, 0.226);
border-radius: 50%;
cursor: pointer;
color: white;
transition: all .4s;
transition-delay: calc(var(--i)* 0.1s);
backdrop-filter: blur(5px);
}
.links a i{
font-size: 1.5em;
}
.container input:checked ~ .links a:nth-child(1){
transform: translateY(-130%);
}
.container input:checked ~ .links a:nth-child(2){
transform: translateX(130%);
}
.container input:checked ~ .links a:nth-child(3){
transform: translateY(130%);
}
.container input:checked ~ .links a:nth-child(4){
transform: translateX(-130%);
}
</style>
</head>
<body>
<div class="container">
<input type="checkbox" name="" id="">
<div class="links">
<a href="#" style="--i:1"><i class="fab fa-facebook"></i></a>
<a href="#" style="--i:2"><i class="fab fa-instagram"></i></a>
<a href="#" style="--i:3"><i class="fab fa-twitter"></i></a>
<a href="#" style="--i:4"><i class="fab fa-whatsapp"></i></a>
</div>
</div>
</body>
</html>
