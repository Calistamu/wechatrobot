# 介绍

想微信自动回复很久，但是发现一搜索只能微信公众号自动回复。想要便利生活，当我做事情时，可以及时礼貌地回复别人。实现了自动回复和陪聊机器人。

# 学习

浅层学习了itchat,了解了什么是wxpy

[我没有那么优秀，站在巨人的肩膀上](https://zhuanlan.zhihu.com/p/30899907?_blank)

学会了使用图灵机器人，大概了解了机器人客服的原理，并使用微信助手清空删除我的好友。

2022-3-26补充：
再次运行这个代码，出现了报错
```
Please scan the QR code to log in.
Please press confirm on your phone.
Traceback (most recent call last):
  File "wechatrobot.py", line 64, in <module>
    itchat.auto_login(enableCmdQR=2, hotReload=True)
  File "C:\Python38\lib\site-packages\itchat\components\register.py", line 31, in auto_login
    self.login(enableCmdQR=enableCmdQR, picDir=picDir, qrCallback=qrCallback,
  File "C:\Python38\lib\site-packages\itchat\components\login.py", line 53, in login
    status = self.check_login()
  File "C:\Python38\lib\site-packages\itchat\components\login.py", line 137, in check_login
    if process_login_info(self, r.text):
  File "C:\Python38\lib\site-packages\itchat\components\login.py", line 172, in process_login_info
    for node in xml.dom.minidom.parseString(r.text).documentElement.childNodes:
  File "C:\Python38\lib\xml\dom\minidom.py", line 1969, in parseString
    return expatbuilder.parseString(string)
  File "C:\Python38\lib\xml\dom\expatbuilder.py", line 925, in parseString
    return builder.parseString(string)
  File "C:\Python38\lib\xml\dom\expatbuilder.py", line 223, in parseString
    parser.Parse(string, True)
xml.parsers.expat.ExpatError: mismatched tag: line 63, column 4
```
参考[问题解决：xml.parsers.expat.ExpatError: mismatched tag: line 63, column 4（itchat）](https://blog.csdn.net/ljhsq/article/details/122756196),该文章是2022-03-10 09:39:50 修改，因此根据作者的解释，这个代码已经废弃了，itchat已经用不了了。再参考[克隆自开源项目ItChat，解决微信帐号不能登录网页版问题](https://gitee.com/lihaitao/ItChat)发现四个月前更新的文章，有了uos这一对itchat的补丁，但是也没有用，所以itchat彻底废了，这个代码已经无法使用。

