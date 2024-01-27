# ConfluenceMemshell
Confluence CVE 2021，2022，2023 利用工具，支持命令执行，哥斯拉，冰蝎 内存马注入
* 支持 Confluence 版本：CVE-2021-26084，CVE-2022-26134，CVE_2023_22515，CVE-2023-22527
* (如果对您有帮助，感觉不错的话，请您给个大大的 ⭐️❗️)
* 哥斯拉默认密码：pass ，默认key：key
* 冰蝎默认密码：rebeyond，默认UA：Accept-Language:zh-CN,zh;q=0.95,n-AS,fr-RF
* 只有 CVE-2022-26134 版本支持哥斯拉，冰蝎自定义密码，其他版本都是默认密码

**V1.1版本**
* 新增 CVE_2023_22515，用户创建，内存马注入，基于 CmdShell 的命令执行
* table 双击复制当前行，shell路径，key，ua
* 哥斯拉 memshell 地址：url+/plugins/servlet/com/atlassian/TeamManageServlet
* 哥斯拉默认密码：pass ，默认key：key
* CmdShell 地址:url+/plugins/servlet/com/atlassian/TeamManageServlet?team=whoami

1. 创建用户

<img width="780" alt="image" src="https://github.com/Lotus6/ConfluenceMemshell/assets/63742814/b360d9c3-3201-4c15-8237-453e55b64194">

* 成功创建
<img width="1389" alt="image" src="https://github.com/Lotus6/ConfluenceMemshell/assets/63742814/ae4d1a0c-bd45-49aa-9107-563898954c4f">

2. 生成恶意插件 Jar 包（包含哥斯拉，和CmdShell）

<img width="785" alt="image" src="https://github.com/Lotus6/ConfluenceMemshell/assets/63742814/3f7c1518-d2f6-4e58-82c2-3d8935def5d0">

* 显示内存马地址，和pass:key（双击复制，shell路径，key，ua）

<img width="788" alt="image" src="https://github.com/Lotus6/ConfluenceMemshell/assets/63742814/621f2e34-4055-48d8-995e-559fdb056ebf">

3. 用创建的用户进后台，插件功能地址： url+/plugins/servlet/upm，上传插件（不用等传完，直接刷新就有了。）

<img width="1021" alt="image" src="https://github.com/Lotus6/ConfluenceMemshell/assets/63742814/694e70af-cd88-4bac-958e-fe4c55d2e414">

4. 哥斯拉连接

<img width="483" alt="image" src="https://github.com/Lotus6/ConfluenceMemshell/assets/63742814/55bbc76a-33cc-466c-b84f-331fa5de6bbd">

5. 基于插件 CmdShell 命令执行
<img width="788" alt="image" src="https://github.com/Lotus6/ConfluenceMemshell/assets/63742814/654ca5a9-85a3-4fdf-b994-06fffc8d10f8">


**V1.0**
1. 命令执行（其他 CVE 版本同理）
  
  <img width="788" alt="image" src="https://github.com/Lotus6/ConfluenceMemshell/assets/63742814/ebbad08a-994c-4717-818a-721f24250119">


2. 内存马注入（其他 CVE 版本同理）
* 哥斯拉

<img width="788" alt="image" src="https://github.com/Lotus6/ConfluenceMemshell/assets/63742814/b7221eaa-d7d5-4fce-ba77-d3f1969b492a">

<img width="477" alt="image" src="https://github.com/Lotus6/ConfluenceMemshell/assets/63742814/0cc1c2cf-b0b8-43f0-8b18-9d3333824cef">

* 冰蝎

<img width="788" alt="image" src="https://github.com/Lotus6/ConfluenceMemshell/assets/63742814/21861463-c3ba-41f5-a7a7-9249758eb8e3">


<img width="1291" alt="image" src="https://github.com/Lotus6/ConfluenceMemshell/assets/63742814/d95dd5c7-6843-4c3c-aac7-bb3147e32005">



**参考**

https://github.com/BeichenDream/CVE-2022-26134-Godzilla-MEMSHELL
https://github.com/aaaademo/Confluence-EvilJar

##

**免责声明**



本工具仅能在取得足够合法授权的企业安全建设中使用，在使用本工具过程中，您应确保自己所有行为符合当地的法律法规。


如您在使用本工具的过程中存在任何非法行为，您将自行承担所有后果，本工具所有开发者和所有贡献者不承担任何法律及连带责任。
