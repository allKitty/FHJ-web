10.21�ղ���
�ڱ��ش���һ���ļ��н�test10.21 ,�ļ�����Ӧ����5��html�ļ�,�ֱ�����Ϊ1.html��.�ٴ���һ��readme.txt�ļ�,���⼸��������������,���html�е�js������������·�.

1.�������ַ������ַ�������ķ������һ���ַ�,��ʾ��ҳ��idΪh1��Ԫ����
��: 
    <h1 id="h1"></h1>
    <script>
       var h1=document.getElementById('h1');
       var s1="��һ�����";
       var s2="�ڶ�������";
       var s3=s1.concat(s2);
       console.log(s3);
       h1.innerHTML=s3;
    </script>

2.һ���������87��,����ƹ���д��87w,���Զ����ɴ洢870000�ķ���,��ʾ��ҳ��idΪh2��Ԫ����
��:  
    <h2 id="h2"></h2>
    <script>
        var h2=document.getElementById('h2');
        var str='87';
        var estr = str.padEnd(6,'0');
        // console.log(estr);
        h2.innerHTML=estr;
        
    </script>

3.һ������79387.348�Ĺ��̿�,������λС������,��ʾ��ҳ��idΪh3��Ԫ����
��:  
    <h3 id="h3"></h3>
    <script>
        var h3=document.getElementById("h3");
        var num=79387.348;
        var num1=num.toFixed(2);
        h3.innerHTML=num1;
    </script>

4.һ��ͼƬ��һ�����·��img/head/,icon/1.jpg,��ֻ��Ҫ�õ������ļ���Ŀ¼����ʾ��ҳ��idΪh4��Ԫ����
��: 
    <h4 id="h4"></h4>
    <img src="img/head/icon/1.jpg" alt="" id="img">
    <script>
        var h4=document.getElementById('h4');
        var img=document.getElementById('img');
        h4.innerHTML=img.src;
    </script>

5.�û�������֤��,���۴�Сд���붼����ȷ�ķ���,��ʾ��ҳ��idΪh1��Ԫ����,��ʾ��ҳ��idΪh4��Ԫ����
��:      
    <h1 id="h1"></h1>
    <script>
       var h1=document.getElementById('h1');
       var yan=prompt('��������֤��:ahJ');
       var yan1='ahJ';
       if(yan1.toLowerCase==yan.toLowerCase()||yan.toUpperCase==yan1.toUpperCase){
           alert("��ȷ");
       }
       h1.innerHTML=yan;
    </script>