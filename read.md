## Fast_vulnerability_verification

需要在poc.json文件中fofa_userna输入fofa用户名， fofa_password输入fofa密码

### 获取帮助

python3 Fast_vulnerability_verification.py -h

![image-20220405190626028](https://s2.loli.net/2022/04/05/8STYLEDQad2MWiz.png)

### 单个URL漏洞验证

python basic.py -u http://125.75.6.2:88

![image-20220405190810290](https://s2.loli.net/2022/04/05/wPmsqFEiY364k2I.png)

### 多个url 漏洞验证

python basic.py -f b.txt

![image-20220405190854589](https://s2.loli.net/2022/04/05/7cwheX3BL2aNbWi.png)

### FOFA漏洞验证

python basic.py -F

![image-20220405191300950](https://s2.loli.net/2022/04/05/ud2kUIGmgqrcoAv.png)

### 使用burpsuit做代理服务器

python basic.py -F -b

![image-20220405192323278](https://s2.loli.net/2022/04/05/rQl8bdfVDMCPe6R.png)

### 不足

1、目前FOFA自动化登录可能存在一定的失败率，可以多运行几次。

2、目前脚本仅支持单一请求，复杂请求需要修改sendRequest模块。

3、该脚本扩展性不是很好，缺少程序设计的思想。

### 参考

https://mp.weixin.qq.com/s/Dwec68-ROfiqWeRUY4wEpg