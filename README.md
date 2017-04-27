# PHPStudy



<head>
    <script src="http://code.jquery.com/jquery-latest.js"></script>
    <script>
        var i=0;
    $(document).ready(function(){
        setInterval('gaibian()',1000);
        });
        function gaibian(){
            if(i==0){
                i=1;
                $("#wo").removeClass("zhuan_left");
                $("#wo").addClass("zhuan_right");
                }else{
                    i=0;
                    $("#wo").addClass("zhuan_left");
                    $("#wo").removeClass("zhuan_right");
                    }
             
            }
    </script>
    <style>
    .zhuan_left{
         transform: rotate(-20deg);
          -webkit-transform: rotate(-20deg);
        }  
    .zhuan_right{
         -webkit-transform: rotate(20deg);
          transform: rotate(20deg);
        }  
 
img {
    transform-origin: 50% 100% 0;
    -webkit-transform-origin: 50% 100% 0;
     -webkit-transition: all 1s ease-in-out 0s;
    -o-transition: all 1s ease-in-out 0s;
    -moz-transition: all 1s ease-in-out 0s;
    transition: all 1s ease-in-out 0s;
}
    </style>
<style>
div{
    background: none repeat scroll 0 0 #9ACD32;
    height: 120px;
    margin: 0 auto;
    text-align: center;
    width: 200px;
}
</style>
</head>
<body>
<div><img width="100px" id='wo' src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1493227564328&di=06e79b6575dbc9465ce92540c386ce4b&imgtype=0&src=http%3A%2F%2Fpic88.nipic.com%2Ffile%2F20160123%2F22530933_123830881000_2.jpg"/></div>
</body>
