# -
汽车公告查询平台，（开发所有工具 yii2 服务端系统，python 数据采集端，vc 应用桌面端）案例见 www.alisw.com
汽车公告查询平台系统是yii2 开发
系统目录:
   首页
   专用车中心
   配件中心
   商家
   报价
   二手信息
   汽车公告桌面端下载

桌面端自动更新升级部署流程：
   1.必须在32系统下编译gonggao.exe  
     编译前修改gonggao.exe 中CGonggaoApp 中BOOL CGonggaoApp::InitInstance() 的Version="1.0";  版本，版本为更新版本号

  2.vv.php 修改中Version="1.0"; 版本为当前版本，此版本号必须大于旧的gonggao.exe  中BOOL CGonggaoApp::InitInstance() 的Version="1.0" 的版本号，便于软件启动触发更新

  3.appupdate.ini 修改此文件中VERSION=1.1版本号，此版本是更新版本号，vv.php是触发更新版本号。
  如果需要更新文件，需要修改FILE0，FILE1，FILE2，...的更新文件

  4.setup 为安装文件，Update.exe为更新升级文件 website.exe 为网站推广优化文件，gonggao.exe为公告查询文件
   
   
   由于近期工作比较忙，本系统还在开发中，等完善后进行开源分享，希望各行家提出意见。
