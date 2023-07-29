# Comparing `tmp/nonebot_plugin_disconnect_notice-0.1.4.tar.gz` & `tmp/nonebot_plugin_disconnect_notice-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_disconnect_notice-0.1.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_disconnect_notice-0.1.5.tar", max compression
```

## Comparing `nonebot_plugin_disconnect_notice-0.1.4.tar` & `nonebot_plugin_disconnect_notice-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-07-24 16:24:22.718401 nonebot_plugin_disconnect_notice-0.1.4/LICENSE
--rw-r--r--   0        0        0     3680 2023-07-24 16:24:22.718401 nonebot_plugin_disconnect_notice-0.1.4/README.md
--rw-r--r--   0        0        0     2497 2023-07-24 16:24:22.718401 nonebot_plugin_disconnect_notice-0.1.4/nonebot_plugin_disconnect_notice/__init__.py
--rw-r--r--   0        0        0      688 2023-07-24 16:24:22.718401 nonebot_plugin_disconnect_notice-0.1.4/nonebot_plugin_disconnect_notice/config.py
--rw-r--r--   0        0        0      784 2023-07-24 16:24:22.718401 nonebot_plugin_disconnect_notice-0.1.4/nonebot_plugin_disconnect_notice/dataClass.py
--rw-r--r--   0        0        0     2099 2023-07-24 16:24:22.722401 nonebot_plugin_disconnect_notice-0.1.4/nonebot_plugin_disconnect_notice/utils.py
--rw-r--r--   0        0        0      445 2023-07-24 16:24:22.722401 nonebot_plugin_disconnect_notice-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4300 1970-01-01 00:00:00.000000 nonebot_plugin_disconnect_notice-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-29 03:19:35.073256 nonebot_plugin_disconnect_notice-0.1.5/LICENSE
+-rw-r--r--   0        0        0     5109 2023-07-29 03:19:35.073256 nonebot_plugin_disconnect_notice-0.1.5/README.md
+-rw-r--r--   0        0        0     2497 2023-07-29 03:19:35.081256 nonebot_plugin_disconnect_notice-0.1.5/nonebot_plugin_disconnect_notice/__init__.py
+-rw-r--r--   0        0        0      688 2023-07-29 03:19:35.081256 nonebot_plugin_disconnect_notice-0.1.5/nonebot_plugin_disconnect_notice/config.py
+-rw-r--r--   0        0        0      784 2023-07-29 03:19:35.081256 nonebot_plugin_disconnect_notice-0.1.5/nonebot_plugin_disconnect_notice/dataClass.py
+-rw-r--r--   0        0        0     2102 2023-07-29 03:19:35.081256 nonebot_plugin_disconnect_notice-0.1.5/nonebot_plugin_disconnect_notice/utils.py
+-rw-r--r--   0        0        0      445 2023-07-29 03:19:35.081256 nonebot_plugin_disconnect_notice-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5729 1970-01-01 00:00:00.000000 nonebot_plugin_disconnect_notice-0.1.5/PKG-INFO
```

### Comparing `nonebot_plugin_disconnect_notice-0.1.4/LICENSE` & `nonebot_plugin_disconnect_notice-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_disconnect_notice-0.1.4/README.md` & `nonebot_plugin_disconnect_notice-0.1.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -56,20 +56,56 @@
     poetry add nonebot-plugin-disconnect-notice
 </details>
 
 </details>
 
 
 ## ⚙️ 配置
-运行插件前，需要在 nonebot2 项目的`.env.prod`文件中添加下表中的代理地址配置项
+运行插件前，需要在 nonebot2 项目的`.env.prod`文件中添加下表中的smtp配置项
+<details>
+<summary>如果没有开启smtp看这里</summary>
+
+- 以qq邮箱为例，其他邮箱的开启smtp方式是类似的
+
+1.点击qq邮箱的设置
+![img.png](images/img.png)
+
+2.点击账户
+![img_1.png](images/img_1.png)
+
+3.点击管理服务，如果没有开启，这里可能显示的是`开启服务`
+![img_2.png](images/img_2.png)
+
+4.点击`生成授权码`
+![img_3.png](images/img_3.png)
+
+5.按照要求用密保手机号发送短信验证
+![img_4.png](images/img_4.png)
+
+6.复制得到的这个授权码
+![img_5.png](images/img_5.png)
+
+7.得到的这个`授权码`就相当于邮箱密码，邮箱账号就是qq邮箱，其他的一些常见邮箱的smtp_server和smtp_port配置参数参考下表
+
+|   邮箱名    |   smtp_server   | smtp_port |   
+|:--------:|:---------------:|:---------:|
+|   qq邮箱   |   smtp.qq.com   |    465    |   
+| 网易yeah邮箱 |  smtp.yeah.net  |    465    |
+|  阿里云邮箱   | smtp.aliyun.com |    465    |
+| 网易163邮箱  |  smtp.163.com   |    465    |
+| 移动139邮箱  |  smtp.139.com   |    465    |
+
+
+</details>
+
 
 | 配置项 | 必填 | 值类型 | 默认值 | 说明 |
 |:------:|:----:|:---:|:---:|:--:|
 | disconnect_notice_smtp_user | 是 | str | ""  | 邮箱账号,如 114514@yeah.net |
-| disconnect_notice_smtp_password | 是 | str | ""  | 邮箱密码,如 114514 |
+| disconnect_notice_smtp_password | 是 | str | ""  | 邮箱密码或授权码,如 114514 |
 | disconnect_notice_smtp_server | 是 | str | ""  | 邮箱服务器地址,如 smtp.yeah.net |
 | disconnect_notice_smtp_port | 是 | int | 465  | 邮箱端口号，ssl模式时为465 |
 | disconnect_notice_notice_email | 是 | str | ""  | 收件人邮箱，填写自己邮箱即可 |
 | disconnect_notice_dev_mode | 否 | bool | False  | 开发者模式，该模式下bot断开连接不会触发通知消息，避免本地测试插件时不断重载而导致的大量掉线通知 |
 
 <details>
 <summary>示例配置</summary>
@@ -77,14 +113,15 @@
 ```env
 # disconnect_notice示例配置
 disconnect_notice_smtp_user = "114514@yeah.net" #邮箱账号
 disconnect_notice_smtp_password = "114514" #邮箱密码
 disconnect_notice_smtp_server = "smtp.yeah.net" #邮箱服务器地址
 disconnect_notice_smtp_port = 465 #邮箱端口号
 disconnect_notice_notice_email = "114514@qq.com" #收件人邮箱
+disconnect_notice_dev_mode = False #开发者模式，该模式下bot断连不会触发通知消息，避免本地测试插件时不断重载而导致的大量掉线通知
 ```
 
 </details>
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ |  范围  |           说明            |
@@ -95,7 +132,12 @@
 <summary>邮件通知</summary>
 
 ![mail.png](images/mail.png)
 
 </details>
 
 ## ✨喜欢的话就点个star✨吧，球球了QAQ
+
+
+## ⏳ Star 趋势
+
+[![Stargazers over time](https://starchart.cc/Cypas/nonebot_plugin_disconnect_notice.svg)](https://starchart.cc/Cypas/nonebot_plugin_disconnect_notice)
```

#### html2text {}

```diff
@@ -10,30 +10,49 @@
 ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-disconnect-notice   ä½¿ç¨åç®¡çå¨å®è£ å¨
 nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
 æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pdm pdm add
 nonebot-plugin-disconnect-notice   poetry poetry add nonebot-plugin-disconnect-
 notice   ## âï¸ éç½® è¿è¡æä»¶åï¼éè¦å¨ nonebot2
-é¡¹ç®ç`.env.prod`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çä»£çå°åéç½®é¡¹ |
-éç½®é¡¹ | å¿å¡« | å¼ç±»å | é»è®¤å¼ | è¯´æ | |:------:|:----:|:---:|:-
---:|:--:| | disconnect_notice_smtp_user | æ¯ | str | "" | é®ç®±è´¦å·,å¦
-114514@yeah.net | | disconnect_notice_smtp_password | æ¯ | str | "" |
-é®ç®±å¯ç ,å¦ 114514 | | disconnect_notice_smtp_server | æ¯ | str | "" |
-é®ç®±æå¡å¨å°å,å¦ smtp.yeah.net | | disconnect_notice_smtp_port | æ¯ |
-int | 465 | é®ç®±ç«¯å£å·ï¼sslæ¨¡å¼æ¶ä¸º465 | |
-disconnect_notice_notice_email | æ¯ | str | "" |
-æ¶ä»¶äººé®ç®±ï¼å¡«åèªå·±é®ç®±å³å¯ | | disconnect_notice_dev_mode | å¦
-| bool | False |
+é¡¹ç®ç`.env.prod`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çsmtpéç½®é¡¹
+å¦ææ²¡æå¼å¯smtpçè¿é -
+ä»¥qqé®ç®±ä¸ºä¾ï¼å¶ä»é®ç®±çå¼å¯smtpæ¹å¼æ¯ç±»ä¼¼ç
+1.ç¹å»qqé®ç®±çè®¾ç½® ![img.png](images/img.png) 2.ç¹å»è´¦æ· !
+[img_1.png](images/img_1.png)
+3.ç¹å»ç®¡çæå¡ï¼å¦ææ²¡æå¼å¯ï¼è¿éå¯è½æ¾ç¤ºçæ¯`å¼å¯æå¡`
+![img_2.png](images/img_2.png) 4.ç¹å»`çæææç ` ![img_3.png](images/
+img_3.png) 5.æç§è¦æ±ç¨å¯ä¿ææºå·åéç­ä¿¡éªè¯ ![img_4.png]
+(images/img_4.png) 6.å¤å¶å¾å°çè¿ä¸ªææç  ![img_5.png](images/
+img_5.png)
+7.å¾å°çè¿ä¸ª`ææç `å°±ç¸å½äºé®ç®±å¯ç ï¼é®ç®±è´¦å·å°±æ¯qqé®ç®±ï¼å¶ä»çä¸äºå¸¸è§é®ç®±çsmtp_serveråsmtp_portéç½®åæ°åèä¸è¡¨
+| é®ç®±å | smtp_server | smtp_port | |:--------:|:---------------:|:--------
+-:| | qqé®ç®± | smtp.qq.com | 465 | | ç½æyeahé®ç®± | smtp.yeah.net | 465 |
+| é¿éäºé®ç®± | smtp.aliyun.com | 465 | | ç½æ163é®ç®± | smtp.163.com |
+465 | | ç§»å¨139é®ç®± | smtp.139.com | 465 |  | éç½®é¡¹ | å¿å¡« |
+å¼ç±»å | é»è®¤å¼ | è¯´æ | |:------:|:----:|:---:|:---:|:--:| |
+disconnect_notice_smtp_user | æ¯ | str | "" | é®ç®±è´¦å·,å¦ 114514@yeah.net
+| | disconnect_notice_smtp_password | æ¯ | str | "" |
+é®ç®±å¯ç æææç ,å¦ 114514 | | disconnect_notice_smtp_server | æ¯ |
+str | "" | é®ç®±æå¡å¨å°å,å¦ smtp.yeah.net | |
+disconnect_notice_smtp_port | æ¯ | int | 465 |
+é®ç®±ç«¯å£å·ï¼sslæ¨¡å¼æ¶ä¸º465 | | disconnect_notice_notice_email | æ¯ |
+str | "" | æ¶ä»¶äººé®ç®±ï¼å¡«åèªå·±é®ç®±å³å¯ | |
+disconnect_notice_dev_mode | å¦ | bool | False |
 å¼åèæ¨¡å¼ï¼è¯¥æ¨¡å¼ä¸botæ­å¼è¿æ¥ä¸ä¼è§¦åéç¥æ¶æ¯ï¼é¿åæ¬å°æµè¯æä»¶æ¶ä¸æ­éè½½èå¯¼è´çå¤§éæçº¿éç¥
 |  ç¤ºä¾éç½® ```env # disconnect_noticeç¤ºä¾éç½®
 disconnect_notice_smtp_user = "114514@yeah.net" #é®ç®±è´¦å·
 disconnect_notice_smtp_password = "114514" #é®ç®±å¯ç 
 disconnect_notice_smtp_server = "smtp.yeah.net" #é®ç®±æå¡å¨å°å
 disconnect_notice_smtp_port = 465 #é®ç®±ç«¯å£å·
-disconnect_notice_notice_email = "114514@qq.com" #æ¶ä»¶äººé®ç®± ```  ## ð
-ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:
-----:|:----:|:----:|:-----------------------:| | æ­è¿éç¥æµè¯ | ä¸»äºº |
-å¦ | ææä¼è¯ |
+disconnect_notice_notice_email = "114514@qq.com" #æ¶ä»¶äººé®ç®±
+disconnect_notice_dev_mode = False
+#å¼åèæ¨¡å¼ï¼è¯¥æ¨¡å¼ä¸botæ­è¿ä¸ä¼è§¦åéç¥æ¶æ¯ï¼é¿åæ¬å°æµè¯æä»¶æ¶ä¸æ­éè½½èå¯¼è´çå¤§éæçº¿éç¥
+```  ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ
+| |:-----:|:----:|:----:|:----:|:-----------------------:| | æ­è¿éç¥æµè¯
+| ä¸»äºº | å¦ | ææä¼è¯ |
 ä¸»å¨è§¦åæçº¿éç¥æµè¯ï¼ç¨æ¥æµè¯éç¥æ¯å¦æ­£å¸¸å¯ç¨ | ###
 ææå¾  é®ä»¶éç¥ ![mail.png](images/mail.png)  ##
-â¨åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§ï¼ççäºQAQ
+â¨åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§ï¼ççäºQAQ ## â³ Star è¶å¿ [!
+[Stargazers over time](https://starchart.cc/Cypas/
+nonebot_plugin_disconnect_notice.svg)](https://starchart.cc/Cypas/
+nonebot_plugin_disconnect_notice)
```

### Comparing `nonebot_plugin_disconnect_notice-0.1.4/nonebot_plugin_disconnect_notice/__init__.py` & `nonebot_plugin_disconnect_notice-0.1.5/nonebot_plugin_disconnect_notice/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_disconnect_notice-0.1.4/nonebot_plugin_disconnect_notice/config.py` & `nonebot_plugin_disconnect_notice-0.1.5/nonebot_plugin_disconnect_notice/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_disconnect_notice-0.1.4/nonebot_plugin_disconnect_notice/dataClass.py` & `nonebot_plugin_disconnect_notice-0.1.5/nonebot_plugin_disconnect_notice/dataClass.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_disconnect_notice-0.1.4/nonebot_plugin_disconnect_notice/utils.py` & `nonebot_plugin_disconnect_notice-0.1.5/nonebot_plugin_disconnect_notice/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         logger.error(error)
         return error
     # 邮件正文
     subject = f"你的bot掉线了"
     content = f"你的 {bot_params.adapter_name} 适配器的bot账号: {bot_params.bot_id} 掉线了，可能是被风控了，赶快去看看吧"
     if test:
         subject = f"掉线通知测试"
-        content = f"这是一封掉线通知测试邮件，你bot并没有掉线"
+        content = f"这是一封掉线通知测试邮件，你的bot并没有掉线"
 
     # 构造邮件内容
     message = MIMEMultipart("alternative")
     message["Subject"] = Header(subject, 'utf-8')
     message["From"] = mail_config.user
     message["To"] = mail_config.notice_email
     message.attach(MIMEText(content))
```

### Comparing `nonebot_plugin_disconnect_notice-0.1.4/PKG-INFO` & `nonebot_plugin_disconnect_notice-0.1.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-disconnect-notice
-Version: 0.1.4
+Version: 0.1.5
 Summary: bot断连时的通知插件
 Author: cypas
 Author-email: ayano05@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -73,20 +73,56 @@
     poetry add nonebot-plugin-disconnect-notice
 </details>
 
 </details>
 
 
 ## ⚙️ 配置
-运行插件前，需要在 nonebot2 项目的`.env.prod`文件中添加下表中的代理地址配置项
+运行插件前，需要在 nonebot2 项目的`.env.prod`文件中添加下表中的smtp配置项
+<details>
+<summary>如果没有开启smtp看这里</summary>
+
+- 以qq邮箱为例，其他邮箱的开启smtp方式是类似的
+
+1.点击qq邮箱的设置
+![img.png](images/img.png)
+
+2.点击账户
+![img_1.png](images/img_1.png)
+
+3.点击管理服务，如果没有开启，这里可能显示的是`开启服务`
+![img_2.png](images/img_2.png)
+
+4.点击`生成授权码`
+![img_3.png](images/img_3.png)
+
+5.按照要求用密保手机号发送短信验证
+![img_4.png](images/img_4.png)
+
+6.复制得到的这个授权码
+![img_5.png](images/img_5.png)
+
+7.得到的这个`授权码`就相当于邮箱密码，邮箱账号就是qq邮箱，其他的一些常见邮箱的smtp_server和smtp_port配置参数参考下表
+
+|   邮箱名    |   smtp_server   | smtp_port |   
+|:--------:|:---------------:|:---------:|
+|   qq邮箱   |   smtp.qq.com   |    465    |   
+| 网易yeah邮箱 |  smtp.yeah.net  |    465    |
+|  阿里云邮箱   | smtp.aliyun.com |    465    |
+| 网易163邮箱  |  smtp.163.com   |    465    |
+| 移动139邮箱  |  smtp.139.com   |    465    |
+
+
+</details>
+
 
 | 配置项 | 必填 | 值类型 | 默认值 | 说明 |
 |:------:|:----:|:---:|:---:|:--:|
 | disconnect_notice_smtp_user | 是 | str | ""  | 邮箱账号,如 114514@yeah.net |
-| disconnect_notice_smtp_password | 是 | str | ""  | 邮箱密码,如 114514 |
+| disconnect_notice_smtp_password | 是 | str | ""  | 邮箱密码或授权码,如 114514 |
 | disconnect_notice_smtp_server | 是 | str | ""  | 邮箱服务器地址,如 smtp.yeah.net |
 | disconnect_notice_smtp_port | 是 | int | 465  | 邮箱端口号，ssl模式时为465 |
 | disconnect_notice_notice_email | 是 | str | ""  | 收件人邮箱，填写自己邮箱即可 |
 | disconnect_notice_dev_mode | 否 | bool | False  | 开发者模式，该模式下bot断开连接不会触发通知消息，避免本地测试插件时不断重载而导致的大量掉线通知 |
 
 <details>
 <summary>示例配置</summary>
@@ -94,14 +130,15 @@
 ```env
 # disconnect_notice示例配置
 disconnect_notice_smtp_user = "114514@yeah.net" #邮箱账号
 disconnect_notice_smtp_password = "114514" #邮箱密码
 disconnect_notice_smtp_server = "smtp.yeah.net" #邮箱服务器地址
 disconnect_notice_smtp_port = 465 #邮箱端口号
 disconnect_notice_notice_email = "114514@qq.com" #收件人邮箱
+disconnect_notice_dev_mode = False #开发者模式，该模式下bot断连不会触发通知消息，避免本地测试插件时不断重载而导致的大量掉线通知
 ```
 
 </details>
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ |  范围  |           说明            |
@@ -113,7 +150,12 @@
 
 ![mail.png](images/mail.png)
 
 </details>
 
 ## ✨喜欢的话就点个star✨吧，球球了QAQ
 
+
+## ⏳ Star 趋势
+
+[![Stargazers over time](https://starchart.cc/Cypas/nonebot_plugin_disconnect_notice.svg)](https://starchart.cc/Cypas/nonebot_plugin_disconnect_notice)
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-disconnect-notice Version: 0.1.4
+Metadata-Version: 2.1 Name: nonebot-plugin-disconnect-notice Version: 0.1.5
 Summary: botæ­è¿æ¶çéç¥æä»¶ Author: cypas Author-email:
 ayano05@outlook.com Requires-Python: >=3.8,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiosmtplib (>=2.0.2,<3.0.0) Requires-Dist: nonebot-adapter-
 onebot (>=2.1.3,<3.0.0) Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Description-
@@ -19,30 +19,49 @@
 ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-disconnect-notice   ä½¿ç¨åç®¡çå¨å®è£ å¨
 nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
 æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pdm pdm add
 nonebot-plugin-disconnect-notice   poetry poetry add nonebot-plugin-disconnect-
 notice   ## âï¸ éç½® è¿è¡æä»¶åï¼éè¦å¨ nonebot2
-é¡¹ç®ç`.env.prod`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çä»£çå°åéç½®é¡¹ |
-éç½®é¡¹ | å¿å¡« | å¼ç±»å | é»è®¤å¼ | è¯´æ | |:------:|:----:|:---:|:-
---:|:--:| | disconnect_notice_smtp_user | æ¯ | str | "" | é®ç®±è´¦å·,å¦
-114514@yeah.net | | disconnect_notice_smtp_password | æ¯ | str | "" |
-é®ç®±å¯ç ,å¦ 114514 | | disconnect_notice_smtp_server | æ¯ | str | "" |
-é®ç®±æå¡å¨å°å,å¦ smtp.yeah.net | | disconnect_notice_smtp_port | æ¯ |
-int | 465 | é®ç®±ç«¯å£å·ï¼sslæ¨¡å¼æ¶ä¸º465 | |
-disconnect_notice_notice_email | æ¯ | str | "" |
-æ¶ä»¶äººé®ç®±ï¼å¡«åèªå·±é®ç®±å³å¯ | | disconnect_notice_dev_mode | å¦
-| bool | False |
+é¡¹ç®ç`.env.prod`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çsmtpéç½®é¡¹
+å¦ææ²¡æå¼å¯smtpçè¿é -
+ä»¥qqé®ç®±ä¸ºä¾ï¼å¶ä»é®ç®±çå¼å¯smtpæ¹å¼æ¯ç±»ä¼¼ç
+1.ç¹å»qqé®ç®±çè®¾ç½® ![img.png](images/img.png) 2.ç¹å»è´¦æ· !
+[img_1.png](images/img_1.png)
+3.ç¹å»ç®¡çæå¡ï¼å¦ææ²¡æå¼å¯ï¼è¿éå¯è½æ¾ç¤ºçæ¯`å¼å¯æå¡`
+![img_2.png](images/img_2.png) 4.ç¹å»`çæææç ` ![img_3.png](images/
+img_3.png) 5.æç§è¦æ±ç¨å¯ä¿ææºå·åéç­ä¿¡éªè¯ ![img_4.png]
+(images/img_4.png) 6.å¤å¶å¾å°çè¿ä¸ªææç  ![img_5.png](images/
+img_5.png)
+7.å¾å°çè¿ä¸ª`ææç `å°±ç¸å½äºé®ç®±å¯ç ï¼é®ç®±è´¦å·å°±æ¯qqé®ç®±ï¼å¶ä»çä¸äºå¸¸è§é®ç®±çsmtp_serveråsmtp_portéç½®åæ°åèä¸è¡¨
+| é®ç®±å | smtp_server | smtp_port | |:--------:|:---------------:|:--------
+-:| | qqé®ç®± | smtp.qq.com | 465 | | ç½æyeahé®ç®± | smtp.yeah.net | 465 |
+| é¿éäºé®ç®± | smtp.aliyun.com | 465 | | ç½æ163é®ç®± | smtp.163.com |
+465 | | ç§»å¨139é®ç®± | smtp.139.com | 465 |  | éç½®é¡¹ | å¿å¡« |
+å¼ç±»å | é»è®¤å¼ | è¯´æ | |:------:|:----:|:---:|:---:|:--:| |
+disconnect_notice_smtp_user | æ¯ | str | "" | é®ç®±è´¦å·,å¦ 114514@yeah.net
+| | disconnect_notice_smtp_password | æ¯ | str | "" |
+é®ç®±å¯ç æææç ,å¦ 114514 | | disconnect_notice_smtp_server | æ¯ |
+str | "" | é®ç®±æå¡å¨å°å,å¦ smtp.yeah.net | |
+disconnect_notice_smtp_port | æ¯ | int | 465 |
+é®ç®±ç«¯å£å·ï¼sslæ¨¡å¼æ¶ä¸º465 | | disconnect_notice_notice_email | æ¯ |
+str | "" | æ¶ä»¶äººé®ç®±ï¼å¡«åèªå·±é®ç®±å³å¯ | |
+disconnect_notice_dev_mode | å¦ | bool | False |
 å¼åèæ¨¡å¼ï¼è¯¥æ¨¡å¼ä¸botæ­å¼è¿æ¥ä¸ä¼è§¦åéç¥æ¶æ¯ï¼é¿åæ¬å°æµè¯æä»¶æ¶ä¸æ­éè½½èå¯¼è´çå¤§éæçº¿éç¥
 |  ç¤ºä¾éç½® ```env # disconnect_noticeç¤ºä¾éç½®
 disconnect_notice_smtp_user = "114514@yeah.net" #é®ç®±è´¦å·
 disconnect_notice_smtp_password = "114514" #é®ç®±å¯ç 
 disconnect_notice_smtp_server = "smtp.yeah.net" #é®ç®±æå¡å¨å°å
 disconnect_notice_smtp_port = 465 #é®ç®±ç«¯å£å·
-disconnect_notice_notice_email = "114514@qq.com" #æ¶ä»¶äººé®ç®± ```  ## ð
-ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:
-----:|:----:|:----:|:-----------------------:| | æ­è¿éç¥æµè¯ | ä¸»äºº |
-å¦ | ææä¼è¯ |
+disconnect_notice_notice_email = "114514@qq.com" #æ¶ä»¶äººé®ç®±
+disconnect_notice_dev_mode = False
+#å¼åèæ¨¡å¼ï¼è¯¥æ¨¡å¼ä¸botæ­è¿ä¸ä¼è§¦åéç¥æ¶æ¯ï¼é¿åæ¬å°æµè¯æä»¶æ¶ä¸æ­éè½½èå¯¼è´çå¤§éæçº¿éç¥
+```  ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ
+| |:-----:|:----:|:----:|:----:|:-----------------------:| | æ­è¿éç¥æµè¯
+| ä¸»äºº | å¦ | ææä¼è¯ |
 ä¸»å¨è§¦åæçº¿éç¥æµè¯ï¼ç¨æ¥æµè¯éç¥æ¯å¦æ­£å¸¸å¯ç¨ | ###
 ææå¾  é®ä»¶éç¥ ![mail.png](images/mail.png)  ##
-â¨åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§ï¼ççäºQAQ
+â¨åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§ï¼ççäºQAQ ## â³ Star è¶å¿ [!
+[Stargazers over time](https://starchart.cc/Cypas/
+nonebot_plugin_disconnect_notice.svg)](https://starchart.cc/Cypas/
+nonebot_plugin_disconnect_notice)
```

