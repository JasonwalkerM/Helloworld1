# Helloworld1
<!DOCTYPE HTML>
<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8">
<title>了不起的盖茨比</title>
<style>
    .boxshow{
        font-family:"miscosoft Yahei";
        text-align:center;
        padding:0;
        color:white;
        font-weight:bold;
        line-height:100px;
        font-size:15px;
        display:block;
        width:200px;
        height:100px;
        background:-webkit-linear-gradient(left,blue,yellow);
        margin-top:10px;
        border-radius:10px;
    }
    .boxshow:hover{
        width:300px;
        height:200px;
        transition:all 0.335s;
        font-size:25px;
        overflow:hidden;
    }
    #box3{
        overflow:hidden;
    }
    #box1:hover{
        background:url("http://img4.imgtn.bdimg.com/it/u=2689285830,2495304056&fm=21&gp=0.jpg");
    }
    #box2:hover{
        background:url(http://img3.imgtn.bdimg.com/it/u=499748262,760539351&fm=21&gp=0.jpg) 300px 200px;
    }
    #box3:hover{
        background:url("http://img0.imgtn.bdimg.com/it/u=3314578736,1324751996&fm=21&gp=0.jpg");
        background-size:300px 200px;
    }
</style>
<script>
    window.onload=function(){
        var boxs=document.getElementById("boxs");
        var boxshow=document.getElementsByTagName("li");
        //alert(boxshow.length);
        //alert("hello world");
        for(var i=0;i<boxshow.length;i++){
            boxshow[i].index=i;
            boxshow[i].onmouseover=function(){
                clearInterval(timer);
               timer=setInterval(
                function(){
                var speed=10;
                if(this.offsetWidth==500){
                    clearInterval(timer);
                }else{
                var this.style.width=speed+this.offsetWidth+"px";
                }
                
            },30)
               
          }
       }
    }
    
</script>
</head>
<body>
<div id="boxs">
   <li id="box1" class="boxshow">Hello this is a new world</li>
    <li id="box2" class="boxshow"></li>
    <li id="box3" class="boxshow"></li>
    <li id="box4" class="boxshow"></li>    
</div>
</body>
</html>
