1.将两个字符利用字符串对象的方法变成一个字符,显示在页面id为h1的元素中
答:
	<h1 id="h1"></h1>
	<script>
		var h1=document.getElementById('h1')
	    var s1 = new String('星期一，');
	    var s2 = new String('好困');
	    var s3 = s1.concat(s2);
	    h1.innerHTML=s3;
    </script>

2.一个富豪想存87万,给理财顾问写了87w,请自动生成存储870000的方法,显示在页面id为h2的元素中
答:
	<h2 id="h2"></h2>
		 <script>
		 	var h2=document.getElementById('h2');
	        var str='87';
	        var estr= str.padEnd(6,'0');
	        h2.innerHTML=estr;
	    </script>

3.一个数字79387.348的工程款,保留两位小数存入,显示在页面id为h3的元素中
答:<h3 id="h3"></h3>
		<script>
			var h3=document.getElementById('h3');
			var a=79387.348;
			var a1=a.toFixed(2);
			h3.innerHTML=a1;
		</script>

4.一张图片是一个相对路径img/head/icon/1.jpg,我只需要拿到它的文件夹目录后显示在页面id为h4的元素中
答:
	<img src="img/head/icon/1.jpg" id="img"/>
		<h4 id="h4"></h4>
		<script type="text/javascript">
			var img=document.getElementById("img");
			var h4=document.getElementById("h4");
			h4.innerHTML=img.src;
		</script>

5.用户输入验证码,无论大小写输入都会正确的方法,显示在页面id为h5的元素中.
答:
	<h5 id="h5"></h5>
		<script>
			var h5=document.getElementById('h5');
			var a=prompt('请输入验证码oASd(不区分大小写)');
			var b=a.toUpperCase();
			if(b=='OASD'){
				h5.innerHTML='正确';
			}
			else{
				h5.innerHTML='验证码错误';
			}
		</script>
