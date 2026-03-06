# khabir-birthday
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Private Access</title>

<style>

body{
background:black;
color:#00ff9c;
font-family:monospace;
padding:30px;
font-size:18px;
}

.cursor{
display:inline-block;
width:10px;
background:#00ff9c;
margin-left:5px;
animation:blink 1s infinite;
}

@keyframes blink{
0%{opacity:1;}
50%{opacity:0;}
100%{opacity:1;}
}

</style>

</head>

<body>

<div id="text"></div><span class="cursor"></span>

<script>

const message = `> System booting...

> Establishing secure connection...
> Connected ✔

> Login required
> Username: MasKhabir
> Password: ********

> Password accepted
> Welcome Mas Khabir ❤️

> Decrypting message from Salwa...
> ██████████ 100%

> Opening message...

> Mas Khabir，生日快乐 🎂

> 谢谢你一直那么努力，
> 也一直那么有责任感。

> 在我心里，
> 你是一个让我很安心的人。

> 希望未来的每一天，
> 你都顺顺利利，
> 也越来越幸福。

> 如果有一天你累了，
> 记得还有我在你身边支持你。

> Final message:
> You have successfully accessed Salwa's heart 🤍

> End of transmission.
`;

let i = 0;
const speed = 35;
const textDiv = document.getElementById("text");

function typeWriter(){
if(i < message.length){
textDiv.innerHTML += message.charAt(i);
i++;
setTimeout(typeWriter, speed);
}
}

typeWriter();

</script>

</body>
</html>
