# birthday-for-logan
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday!</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

body{
    font-family:Arial, Helvetica, sans-serif;
    background:linear-gradient(135deg,#ff9ecf,#ffd1dc,#fff2b2);
    overflow:hidden;
    height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;
}

.container{
    text-align:center;
    z-index:5;
    padding:20px;
}

h1{
    font-size:clamp(2.5rem,8vw,4rem);
    color:white;
    text-shadow:3px 3px 8px rgba(0,0,0,.3);
}

h2{
    margin-top:15px;
    font-size:clamp(1.2rem,4vw,2rem);
    color:white;
}

p{
    margin-top:20px;
    color:white;
    font-size:1.1rem;
}

/* Balloons */

.balloon{
    position:absolute;
    bottom:-150px;
    font-size:50px;
    animation:floatUp linear infinite;
}

.balloon:nth-child(1){
    left:10%;
    animation-duration:12s;
}

.balloon:nth-child(2){
    left:30%;
    animation-duration:10s;
}

.balloon:nth-child(3){
    left:55%;
    animation-duration:13s;
}

.balloon:nth-child(4){
    left:80%;
    animation-duration:9s;
}

@keyframes floatUp{
    from{
        transform:translateY(0);
    }
    to{
        transform:translateY(-120vh);
    }
}

/* Dog */

.dog{
    position:absolute;
    bottom:15px;
    right:-120px;
    font-size:70px;
    animation:walk 14s linear infinite;
    z-index:10;
}

@keyframes walk{
    0%{
        right:-120px;
        transform:scaleX(1);
    }

    100%{
        right:110%;
        transform:scaleX(1);
    }
}

/* Sparkles */

.sparkle{
    position:absolute;
    color:white;
    animation:twinkle 3s infinite;
    opacity:.7;
}

@keyframes twinkle{
    0%,100%{
        transform:scale(.4);
        opacity:.2;
    }

    50%{
        transform:scale(1.2);
        opacity:1;
    }
}

.footer{
    position:absolute;
    bottom:95px;
    width:100%;
    text-align:center;
    color:white;
    font-size:1rem;
}

/* Mobile */

@media(max-width:600px){

.dog{
    font-size:55px;
}

.balloon{
    font-size:40px;
}

.footer{
    font-size:.9rem;
}

}

</style>

</head>

<body>

<div class="container">
<h1>🎉 Happy Birthday! 🎂</h1>

<h2>youre weird but its okay because thats normal</h2>

<p>
may monster energy notice you
giving you free lifetime supply of white monster
</p>
</div>

<div class="footer">
have fun, be dumb, dont die.
</div>

<div class="balloon">🎈</div>
<div class="balloon">🎈</div>
<div class="balloon">🎈</div>
<div class="balloon">🎈</div>

<div class="dog">🐕</div>

<span class="sparkle" style="top:10%;left:20%;font-size:25px;">✨</span>
<span class="sparkle" style="top:20%;left:70%;font-size:20px;">✨</span>
<span class="sparkle" style="top:35%;left:45%;font-size:30px;">⭐</span>
<span class="sparkle" style="top:65%;left:15%;font-size:25px;">✨</span>
<span class="sparkle" style="top:75%;left:80%;font-size:20px;">⭐</span>
<span class="sparkle" style="top:55%;left:60%;font-size:30px;">✨</span>

</body>
</html>