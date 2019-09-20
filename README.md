DCS JSTARS System
===============

Is is a online mission coordinator website for Multiplayers in DCS World.
> Require PHP version > 5.6. suggest higher than version 7.

 + A light weight PHP framework is used: Thinkphp v5.1 (https://github.com/top-think/framework)
 + Framework official site: http://thinkphp.cn/
 + Framework doc: https://www.kancloud.cn/manual/thinkphp5_1/353946 , no Eng version but no worry, use chrome to translate it to eng, there is only small amout of Chinese in it, most of them are code, very ez to understand.

## How to run
> In test env, make sure PHP interpreter is installed.
> clone the project, go to public folder, command line excute php -S localhost:8888  router.php
> OLY DO THAT IN TEST envoirnment, dont put it on internet, suggest use UPUPW http server(https://sourceforge.net/projects/upupw/files/ANK/UPUPW_ANK_W64_V1.1.7.exe/download) or others real HTTP server, if u need to publish it to public.

## Database required
> support MySQL database and mongodb，
> DB config file locate at /config/database.php, change password and stuff if needed,
> SQL file need to be import to database before run, locate in root folder. File name: tp5.sql
> Good to run(open url in browser:localhost:8888)
> Two sample page,1. localhost:8888 2.localhost:8888/index/index/obj_detail


> further config required, i will keep update in this readme Doc.


`一个针对DCS world线上对战的玩家任务分配管理平台

> router.php用于php自带webserver支持，可用于快速测试,注意务必只能使用于开发环境，否则使用正常的HTTP服务器，建议使用UPUPW
> 导入位于根目录的tp5.sql文件到数据库
> 切换到public目录后，启动命令：php -S localhost:8888  router.php
> 上面的目录结构和名称是可以改变的，这取决于你的入口文件和配置参数。



## 命名规范

`ThinkPHP5`遵循PSR-2命名规范和PSR-4自动加载规范，并且注意如下规范：

### 目录和文件

*   目录不强制规范，驼峰和小写+下划线模式均支持；
*   类库、函数文件统一以`.php`为后缀；
*   类的文件名均以命名空间定义，并且命名空间的路径和类库文件所在路径一致；
*   类名和类文件名保持一致，统一采用驼峰法命名（首字母大写）；

### 函数和类、属性命名
*   类的命名采用驼峰法，并且首字母大写，例如 `User`、`UserType`，默认不需要添加后缀，例如`UserController`应该直接命名为`User`；
*   函数的命名使用小写字母和下划线（小写字母开头）的方式，例如 `get_client_ip`；
*   方法的命名使用驼峰法，并且首字母小写，例如 `getUserName`；
*   属性的命名使用驼峰法，并且首字母小写，例如 `tableName`、`instance`；
*   以双下划线“__”打头的函数或方法作为魔法方法，例如 `__call` 和 `__autoload`；

### 常量和配置
*   常量以大写字母和下划线命名，例如 `APP_PATH`和 `THINK_PATH`；
*   配置参数以小写字母和下划线命名，例如 `url_route_on` 和`url_convert`；

### 数据表和字段
*   数据表和字段采用小写加下划线方式命名，并注意字段名不要以下划线开头，例如 `think_user` 表和 `user_name`字段，不建议使用驼峰和中文作为数据表字段命名。

## 参与开发
请参阅 [ThinkPHP5 核心框架包](https://github.com/top-think/framework)。

## 版权信息

ThinkPHP遵循Apache2开源协议发布，并提供免费使用。

本项目包含的第三方源码和二进制文件之版权信息另行标注。

版权所有Copyright © 2006-2018 by ThinkPHP (http://thinkphp.cn)

All rights reserved。

ThinkPHP® 商标和著作权所有者为上海顶想信息科技有限公司。

更多细节参阅 [LICENSE.txt](LICENSE.txt)
