<!DOCTYPE  html>
<html>
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta charset="utf-8">
  <script type="text/javascript">
    function startTime()
    {
    var today=new Date();
    var h=today.getHours();
    var m=today.getMinutes();
    var s=today.getSeconds();
    // add a zero in front of numbers<10
    m=checkTime(m);
    s=checkTime(s);
    document.getElementById('txt').innerHTML=h+":"+m+":"+s;
    t=setTimeout('startTime()',500);
    }
    function checkTime(i)
    {
    if (i<10)
    {
    i="0" + i;
    }
    return i;
    }
    </script>
<title> Hyprx Stargazer</title>
<link rel="shortcut icon" href="Hypricon.ico" /><bgsound src="t2.mp3" loops="1"/>
<script type="text/javascript">
function startTime()
{
var today=new Date();
var h=today.getHours();
var m=today.getMinutes();
var s=today.getSeconds();
// add a zero in front of numbers<10
m=checkTime(m);
s=checkTime(s);
document.getElementById('time').innerHTML=h+":"+m+":"+s;
t=setTimeout('startTime()',500);
}
function checkTime(i)
{
if (i<10)
{
i="0" + i;
}
return i;
}
</script>

<style>
form {
        background-color: #313032bf;
        width: 200px;
        height: 50px;
        border-radius: 50px;
        display:flex;
        flex-direction:row;
        align-items:center;
padding: 4px
      }

      input {
        all: unset;
        font: 16px segoe ui;
        color: #1f1d93;
        height: 100%;
        width: 100%;
        padding: 6px 10px;
      }

      ::placeholder {
        color: rgba(81, 211, 234, 0.905);
      }

      svg {
        color: #1f1d93;
        fill: #1f1d93;
        width: 24px;
        height: 24px;
        padding: 10px;
      }

      button {
        all: unset;
        cursor: pointer;
        width: 60px;
        height: 60px;
      }
* {
margin: 0;
padding: 0;
}

body {
background-size: cover;
}

nav {
width: 100%;
height: 150px;
background-image: linear-gradient(150deg,#1f1d93 , rgba(81, 211, 234, 0.905),purple);
border-radius: 10px 10px 40px 40px ;
}

nav ul {
float: left;
}

nav ul li {
float: left;
list-style: none;
border-radius: 40px;
}
nav ul li:hover {
float: left;
list-style: none;
border-radius: 40;
background-color: #313032bf;
}
nav ul li ul {
display: none;
position: absolute;
background-image: linear-gradient(70deg,rgba(81, 211, 234, 0.905) ,purple);
border-radius: 5px;
}
nav ul li:hover ul {
display:block;
border-radius: 10px 10px 40px 40px;


}

nav ul li ul li {
border-radius: 10px 10px 40px 40px;
padding: 20px;
}
nav ul li ul li a:hover {
background-color: #313032bf;
border-radius: 10px 10px 40px 40px;
}
nav ul li ul div {
background-color: #1f1d93;
}
#mydiv {
  position: absolute;
  z-index: 9;
  background-color: #1f1d93;

  border: 1px solid #1f1d93;
}

#mydivheader {
  padding: 1px;
  cursor: move;
  z-index: 10;
  background-color: #1f1d93;
  color: #313032bf;
}

nav ul li ul li div {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  text-decoration-color: #ffffff;
}
#hs {
  background: linear-gradient(70deg,#1f1d93 , rgba(81, 211, 234, 0.905),purple);
        background-clip: text;
        -webkit-text-fill-color: transparent;
        -webkit-background-clip: text;
}


    </style>

 </head>
<body onload="startTime()">
  <style>
  body {
    background-image: url('https://i0.wp.com/windowscustomization.com/wp-content/uploads/2019/04/Blue-Nebula.gif?fit=768%2C432&quality=80&strip=all&ssl=1');
    background-repeat: no-repeat;
    background-size: 100%;
  }
  </style>
  <script type="text/javascript">
    var clockElement = document.getElementById('clock');

    function clock() {
        clockElement.textContent = new Date().toString();
    }

    setInterval(clock, 1000);
</script>

 <nav >
<ul>
<li><a href="Typer.html"><img src="Hypericon.png" height="150" width="150" ></a>  </li> 
<li><A href= "Images.html"><img src="Himagesicon.png" height="150" width="150" >  </a> </li>
<li> <A href= "Browser.html"><img src="Hrowsericon.png" height="139" width="150"> </a></li>
<li> <A href="User manual.html"> <IMG src="Hrousericon.png" height="150" width="150"> </a></li>
<li><A href="Clock.html"><img src="Hlockicon.png" height="150" width="165"></A></li>

<li><form role="search" id="form">
      <input type="search" id="query" name="q" placeholder="Hyprx Search" aria-label="Search through site content">
      <button>
        <svg viewBox="0 0 1024 1024"><path class="path1" d="M848.471 928l-263.059-263.059c-48.941 36.706-110.118 55.059-177.412 55.059-171.294 0-312-140.706-312-312s140.706-312 312-312c171.294 0 312 140.706 312 312 0 67.294-24.471 128.471-55.059 177.412l263.059 263.059-79.529 79.529zM189.623 408.078c0 121.364 97.091 218.455 218.455 218.455s218.455-97.091 218.455-218.455c0-121.364-103.159-218.455-218.455-218.455-121.364 0-218.455 97.091-218.455 218.455z"></path></svg>
      </button>
    </form>
    <script>
      const f = document.getElementById('form');
      const q = document.getElementById('query');
      const bing = 'https://www.bing.com/search?q=';
      const site = ' ';

      function submitted(event) {
        event.preventDefault();
        const url = bing + site + '+' + q.value;
        const win = window.open(url, '_blank');
        win.focus();
      }

      f.addEventListener('submit', submitted);
    </script> </li>
<li><a href="#"><img src="Hypricon.png" height="150" width="150"></a> 
<ul>
<li> <A href="Typer.html"><img src="Hypericon.png" height="50" width="50" > </A></li>
<li><A href= "Images.html"><img src="Himagesicon.png" height="50" width="50" >  </a> </li>
<li> <A href= "Browser.html"><img src="Hrowsericon.png" height="46.5" width="52.5"> </a></li>
<li> <A href="User manual.html"> <IMG src="Hrousericon.png" height="50" width="50"> </a></li>
<li> <A href="Simpleview.html"> <IMG src="Simplicon.png" height="50" width="50"> </a></li>
<li> <h3><font face="segoe ui"><b><div id="time"></div></b> </h3> </font></li>
<li><div id="txt"></div></li>
</ul>
</li>

</ul>
</nav><br>



<FONT size="200" color="black" face="Segoe UI" id="hx"><b id="hs"> Hyprx Stargazer</b><a href="Abthxs.html"><IMG src="Hypricon.png"height="50" width="50"></a> </font> 
 
 <script type="text/javascript">
  var clockElement = document.getElementById('clock');

  function clock() {
      clockElement.textContent = new Date().toString();
  }

  setInterval(clock, 1000);
</script>

<A href="Intro.html"> <A href="Intro.html"> <IMG src="Hupdatesicon.png"height="100" width="100"> </A>
  

</h2></b> 
<br><br><br><br><br><br><br><br><br><br><br><br><b<br><br><br><br><br><br><br><br><br><br>
<h5><font  face="Segoe UI">Only the Home page is customized.All apps have the default GL color.</font></h5>

</body>
</html> 

