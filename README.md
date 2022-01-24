# kuba.


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        body{margin:0;padding:0}
        img{
            position:absolute;
            top:100px;left:100;
        }
    </style>
</head>
<body>
    <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQokSWICGpmYogpA5UVMDZ3QmaWt-rC4gIfJA&usqp=CAU" width="600" height="600" alt="Planets" usemap="#planetmap" onmousemove="coordinate(event)">
    <map name="planetmap">
        <area shape="rect" coords="34,44,270,350"onmouseover="show('ręka')"  onmouseleave="show('')" alt="ręka" >       
        <area shape="circle" coords="272,120,50" onmouseover="show('głowa')" onmouseleave="show('')" alt="głowa">
        <area shape="circle" coords="361,589,50" onmouseover="show('noga')"  onmouseleave="show('')"alt="noga">
    </map>
    <script>
        // function coordinate(event){
            console.log(event.clientX,event.clientY)
        }
        function show(what){
            const info = document.getElementById('info')
            info.innerHTML = what;
        }
    </script>
</body>
</html>

