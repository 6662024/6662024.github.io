`Gmeek-html<div id="announcement"></div>`
源码说明
AMATAK多语言交易所源码/15种语言+修复k线+平台币行情控制+合约+秒合约+期权+币币交易+永续合约/前端uniapp+后端PHP

测试反馈
测试环境：Linux系统CentOS7.6、宝塔面板、Nginx、PHP7.3、MySQL5.7，运行目录public，伪静态选择laravel5，建议开启SSL

语言：15种，看图

这套就是BitWell的修复版，主要是修复了k线，现在k线正常启动不会掉线，之前发布的那套程序会存在websocket掉线，导致k线不会实时更新

前后端有一定的调整，注释掉了OTC和矿机的功能，需要的话可以对比之前的版本或者在前端启用

前端h5和pc都是纯源码，后端laravel5框架也是开源的，有完整的代理端，后台可以预设平台币的k线行情，结算这些都没问题

这些交易所有几个php混淆加密后门，都是workerman运行时会执行的，使用批量搜索 ;$b11st=0; 将搜索到的文件打开，把加密的这一段删掉 ;$b11st=0; 开始 ;$b11ed=0; 结束
主要文件路径如下：
/vendor/workerman/workerman/Worker.php
/vendor/laravel/framework/src/Illuminate/Foundation/Application.php
/vendor/webmsgsender/vendor/workerman/workerman/Worker.php

而且我发现一个非常严重的问题，就是你在很多论坛程序里面搜索 ;$b11st=0; 大多数程序文件都会有（不信你试试），也不知道是哪个傻逼搞的，自己拿到程序还是得先扫几遍在运行，免得网站被上线了
![image](https://github.com/user-attachments/assets/240a6e48-5d0e-43a6-931b-105e9dda9a0c)
![image](https://github.com/user-attachments/assets/846a0705-96a0-4a20-bcad-381210d870a9)
![image](https://github.com/user-attachments/assets/5319ced1-d64d-4609-bd3e-0d6f2213e34f)
![image](https://github.com/user-attachments/assets/e4502b02-3ada-412c-bad9-9917e9757a50)
![image](https://github.com/user-attachments/assets/8eb1704f-3d70-48d6-be62-f2dae5d0c819)
![image](https://github.com/user-attachments/assets/1355a7a1-496d-4480-9afd-aa0f99dd97ad)
![image](https://github.com/user-attachments/assets/bd67a2c2-b9d2-42f4-9f91-4126bc42c9e0)
![image](https://github.com/user-attachments/assets/6bfbad1b-6bf9-44cc-bfea-c83bade1c15b)
![image](https://github.com/user-attachments/assets/83c535b2-6bea-46d7-875e-1e2233180acd)
![image](https://github.com/user-attachments/assets/4338a163-8e5c-4bc5-8595-36e999163c30)
![image](https://github.com/user-attachments/assets/e61bdbff-3aa9-44af-9044-ac193480ade9)
![image](https://github.com/user-attachments/assets/67bdccc9-b26b-410d-8774-406f3d4c2256)
![image](https://github.com/user-attachments/assets/1164d4ed-c7b4-430e-a45a-f029c9623695)
![image](https://github.com/user-attachments/assets/fe014c27-bb10-4878-8f6d-761489127689)
![image](https://github.com/user-attachments/assets/b52ed9bf-79c2-4048-a72a-dc6d7ad65b71)
![image](https://github.com/user-attachments/assets/f8949987-9edb-46bd-9df5-5a8cd23ddfd9)
![image](https://github.com/user-attachments/assets/a7a2e2b4-b35e-45e5-9afb-fb11089831df)
代理端
![image](https://github.com/user-attachments/assets/3e98c88d-d556-4f4c-aab4-47aae8b386e3)
![image](https://github.com/user-attachments/assets/ad38e2d6-c4b3-4cd7-b31b-d99c3e19a824)
![image](https://github.com/user-attachments/assets/15530238-73b1-4797-bb95-bd00d56aea27)

后台
![image](https://github.com/user-attachments/assets/fbae2a8e-6fb9-425d-a14c-1be55a33031a)
![image](https://github.com/user-attachments/assets/3722fc25-1f11-4e9b-8781-aa157d9a3c1a)
![image](https://github.com/user-attachments/assets/8ce71921-cb1a-4161-ad2f-dac33226e448)
![image](https://github.com/user-attachments/assets/5b7dc3d2-2786-4ed3-b474-5ee4e0a6ea98)
![image](https://github.com/user-attachments/assets/72e743f3-9390-4726-b610-78a5d75d9a9e)
![image](https://github.com/user-attachments/assets/7850f190-57e2-4618-a836-50b1a253a1c1)
![image](https://github.com/user-attachments/assets/7efc0dd8-3025-4bdb-9c24-525103a5ee65)
![image](https://github.com/user-attachments/assets/e0a03e72-c628-4fa5-833f-57c276c83b1b)
![image](https://github.com/user-attachments/assets/859c68bc-e573-40ef-997e-9d00690ee390)
![image](https://github.com/user-attachments/assets/65f991b2-c76a-4654-b8e3-05403c4631f8)
![image](https://github.com/user-attachments/assets/c1bb226d-fc45-46f6-a050-5915596b7f2b)
![image](https://github.com/user-attachments/assets/12505947-4a11-47cb-af09-3493eccea93e)











