# byeTyp
再见typecho！此插件将帮助你将typecho上的资源无缝迁移到WordPress上。

## 安装方法
请移步[https://github.com/ibadboy-net/ByeTyp/releases](https://github.com/ibadboy-net/ByeTyp/releases)，下载当前最新版的插件，并安装到你的Typecho上。

## 使用方法
在Typecho上启用插件后，依次点击：控制台->数据导出->导出XML文件，下载并保存此文件。
在WordPress上运行WordPress导入工具，导入前面下载的XML文件。
WordPress导入工具的运行方法见下图：
![image](https://github.com/ibadboy-net/ByeTyp/images/wp.png)

## 后续步骤
在数据库中替换图片资源路径，执行以下SQL语句：
'''sql
UPDATE wp_posts SET post_content = REPLACE( post_content, '/usr/uploads/', '/wp-content/uploads/');
'''

## 关于问题
有任何问题请移步[https://github.com/ibadboy-net/ByeTyp/issues](https://github.com/ibadboy-net/ByeTyp/issues)提出，我会及时解决的。

## 附加说明
此项目基于[TypExport](https://github.com/panxianhai/TypExport)项目二次开发并提供长期维护。