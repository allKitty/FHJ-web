10.21日测验
在本地创建一个文件夹叫test10.21 ,文件夹中应含有5个html文件,分别命名为1.html等.再创建一个readme.txt文件,将这几个问题贴如其中,最后将html中的js代码贴到答的下方.

1.将两个字符利用字符串对象的方法变成一个字符,显示在页面id为h1的元素中
答: 
    <h1 id="h1"></h1>
    <script>
       var h1=document.getElementById('h1');
       var s1="第一个你好";
       var s2="第二个在吗";
       var s3=s1.concat(s2);
       console.log(s3);
       h1.innerHTML=s3;
    </script>

2.一个富豪想存87万,给理财顾问写了87w,请自动生成存储870000的方法,显示在页面id为h2的元素中
答:  
    <h2 id="h2"></h2>
    <script>
        var h2=document.getElementById('h2');
        var str='87';
        var estr = str.padEnd(6,'0');
        // console.log(estr);
        h2.innerHTML=estr;
        
    </script>

3.一个数字79387.348的工程款,保留两位小数存入,显示在页面id为h3的元素中
答:  
    <h3 id="h3"></h3>
    <script>
        var h3=document.getElementById("h3");
        var num=79387.348;
        var num1=num.toFixed(2);
        h3.innerHTML=num1;
    </script>

4.一张图片是一个相对路径img/head/,icon/1.jpg,我只需要拿到它的文件夹目录后显示在页面id为h4的元素中
答: 
    <h4 id="h4"></h4>
    <img src="img/head/icon/1.jpg" alt="" id="img">
    <script>
        var h4=document.getElementById('h4');
        var img=document.getElementById('img');
        h4.innerHTML=img.src;
    </script>

5.用户输入验证码,无论大小写输入都会正确的方法,显示在页面id为h1的元素中,显示在页面id为h4的元素中
答:      
    <h1 id="h1"></h1>
    <script>
       var h1=document.getElementById('h1');
       var yan=prompt('请输入验证码:ahJ');
       var yan1='ahJ';
       if(yan1.toLowerCase==yan.toLowerCase()||yan.toUpperCase==yan1.toUpperCase){
           alert("正确");
       }
       h1.innerHTML=yan;
    </script>