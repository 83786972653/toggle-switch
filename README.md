<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        body{
            background-color:white;
        }#btn{
            cursor:pointer;
            height:40px;
            width:160px;
            background-color:red;
            font-size:20px;
            font-weight:900;
            font-family:'Courier New',Courier,monospace;
            border: 2px solid white;
            transition-duration: .5s;
        }
        #btn:hover{
            transform:scale(1.1);
        }
        .center{
            text-align:center;
            display:flex;
            justify-content:center;
            align-items:center;
            margin:auto;
            flex-direction:column;
            padding-top:60px;
        }
    </style>
</head>
<body>
    <div class="center">
        <img src="C:\Users\sp524\OneDrive\Desktop\FSI\bulb on & off\bulb off.jpeg" alt="bulb" id="imgon">
        <button id="btn">Turn on</button>
        <script>
            let btn =document.getElementById('btn')
            let img =document.getElementById('imgon')
            btn.addEventListener('click',change)
            function change(e){
                if(btn.textContent.includes('on')){
                    img.src ="bulb on.jpeg"
                    btn.style.backgroundColor = "green"
                    btn.textContent = "Turn off"
                }
                else{
                    img.src="bulb off.jpeg"
                    btn.textContent="Turn on"
                    btn.style.backgroundColor = "red"
                }
            }
        </script>
</body>
</html>![bulb on](https://github.com/83786972653/toggle-switch/assets/157817828/50da51ad-acb8-4d37-b133-9b96edf20280)
![bulb off](https://github.com/83786972653/toggle-switch/assets/157817828/81e83cc8-bc8a-4945-a7ee-9b5d52124119)
