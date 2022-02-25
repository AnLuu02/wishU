<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JS</title>
</head>
<script>
    function bam(){
        document.getElementById("love").style.display = "block";
        document.getElementById("clc").style.display="none";
        document.getElementById("clcc").style.display="none";
    }

    
    function re_chuot(obj){
        obj.innerHTML = "💖Đồng ý💖"
    }

    function re_chuot1(obj){
        obj.innerHTML = "😢Từ chối😢"
    }
</script>
<style>
    .love{
        color: purple;
        display: none;
        font-size: 50px;
        margin-top: 50px;
        margin-left: 15%;
    }
    .body{
        margin: auto;
        margin-top: 200px;
        width: 600px;
        height: 300px;
        box-shadow: rgba(0, 0, 0, 0.4) 0px 0px 10px;
        position: relative;
        background-image: url(/img/nen.jpg);
    }
    .click{
        width: 250px;
        box-shadow: rgba(0, 0, 0, 0.4) 0px 0px 10px;
        /* margin-top: 20%; */
        
    }
    .but{
        font-size: 30px;width: 200px;background-color: pink; color: black;
        position: absolute;
        bottom: 20px;
    }
    button:hover{
        color: black;
        background-color: whitesmoke;
    }
    .container{
        display: flex;
        justify-content: space-around;
    }
</style>
<body background="/img/vlt.png" style="background-size: cover;">
    <audio autoplay src="./audio/audio1.mp3" ></audio>
    <div class="body">
        <marquee width="100%" behavior="alternate" bgcolor="pink" style="font-size: 50px;">😍Hello con c!!😍</marquee>
        <div class="container">
            <div id="clc" class="click"><button onclick="bam()" class="but" style=" width: 250px;">💖Đồng ý💖</button></div>
            <div id="clcc" class="click"><button onclick="bam()" onmouseover="re_chuot(this)" onmouseout="re_chuot1(this)" class="but" style=" width: 250px;">😢Từ chối😢</button></div>
        </div>
        <div id="love" class="love">Cai l!😍❤❤🤣</div>
    </div>
</body>
</html>
