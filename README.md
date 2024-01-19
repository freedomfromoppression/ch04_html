# ch04_html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>z-index</title>
    <style>
        div{position: absolute;}
        img{position: absolute;}
        #img1{z-index: -1;}
        #img2{z-index: -1;left:50px;top: 50px;}
        
    </style>
</head>
<body>
    <h1>z-index 앞 뒤에 위치시키기</h1>
    <h>
    <div>
        <img src="./img/apple.PNG" id="img1"width="100px"height="100px">
        <img src="./img/banana.PNG"id="img2"width="100px"height="100px">
    </div>    
    <ul>
        <li><a href="#">홈</li></a>
        <li><a href="#">메뉴1</li></a>
        <li><a href="#">메뉴2</li></a>
        <li><a href="#">메뉴3</li></a>
    </ul>
    
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        ul{margin:0; padding:0;list-style: none;}/*ul 태그 속성(점) 제거*/
        li{display: inline;}
        ul li a {text-decoration: none;  /*밑줄 제거 a 태그 특성 */
        color: #000;
        padding: 5px 10px;
        }
    ul li a:hover{background-color: #eee;}
    ul li a:active{background-color: gray;}

    </style>
</head>
<body>
    <ul>
        <li><a href="#">홈</a></li>
        <li><a href="#">메뉴1</a></li>
        <li><a href="#">메뉴2</a></li>
        <li><a href="#">메뉴3</a></li>
    
</body>
</html>


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>애니메이션</title>
    <style>
        /*애니메이션 정의 */
        @keyframes bomb {0% {font-size: 100%;}
                        50% {font-size: 500%;}
                        100% {font-size: 100%;} 
        }
        @keyframes colorchange {from{color: blue;}
                                 to{color: red}            
        }
        h1{animation-name:boom;animation-duration 3s;
            animation-iteration-count:infinite;}
        h2{animation-name:colorchange;animation-duration 2s;
            animation-iteration-count:infinite;}
                
    </style>
</head>
<body>
    <h2>색변경</h2>
    <h1>꽝</h1>
    <hr>
    <p>글자가 10초동안 바뀜</p>
    
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>전환</title>
    <style>
        span{transition: font-size 5s,color 5s margin-left 1s;}
        span:hover {font-size: 500%,; color:red}
        span:active{margin-left: 100px;}
    </style>
</head>
<body>
    <h3>font-size에 대한 전환</h3>
    <hr>
    <p><span>꽝</span>글자에 마우스를 올리면 전환됨.</p>
    
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>전환2</title>
    <style>
        #rec{width: 100px; height: 200px;background-color: red;transition-duration: 0.6s;}
        #rec{width: 150px;height: 100px;background-color: green;}
        #rec:active{width: 150px ;height: 100px;background-color: blue;border-radius: 100px;}
    </style>
</head>
<body>
    <div id="warp">
        <div id="rec"></div>
    </div>
    
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>변환</title>
    <style>
        #ex{position: relative;width: 500px;height: 150px;margin: 0;border: 1px solid aquamarine;}
        .box{font-size: 12px;position: relative;width: 60px;height: 60px;margin-bottom:10px;background-color: #eee;}
        .box p{text-align: center;padding-top: 4px;}
        #ex:hover .box{transform: rotate(720deg);margin-left: 420px;}
        #no-delay{transition-duration: 3s;border: 1px solid orange;}
        #delay{transition-duration: 3s;transition-delay: 1s;border: 1px solid blue; }
    </style>
</head>
<body>
    <div id="ex">
        <div id="no-delay" class="box"><p>no-delay</p></div>
        <div id="delay" class="box"><p>delay</p></div>

    </div>
    
</body>
</html>
