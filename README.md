# curl-number-bash
this can be used in htb tenten 

for i in $(seq 1 20); do echo -n "$i: "; curl -s http://10.10.10.10/index.php/jobs/apply/$i/ | grep '<title>'; done

如果一个网页地址，某处不同的数字编号，就会进入不同的网页界面。显示出不同的新的一些标题。

这个小脚本。可以用来跑，免得一个个手打试。最后grep抓取出不同的标题。

也可根据其他不同的情况做些修改。
