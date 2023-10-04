#   Linux：在Linux世界，一切皆文件！ 

## 1、思维导图
![输入图片说明](pictures/_Linux%E5%9F%BA%E7%A1%80_Ruchine.png)  

## 2、知识点摘要

### 常用基本命令

####  【1】文件目录类
- 熟悉目录结构，熟悉各文件夹主要功用  
- 熟悉文件目录指令： **pwd** 、 **ls** 、 **cd** 、 **mkdir** 、 **rmdir** 、 **touch** 、 **cp** 、 **rm** 、 **mv** 、 **cat** 、 **more** 、 **less** 、 **echo** 、 **head** 、 **tail** 、 **history** 

#### 【2】时间日期类
- 熟悉时间日期指令： **date** 、 **cal** 

#### 【3】用户管理类
- 熟悉用户管理指令： **useradd** 、 **passwd** 、 **userdel** 、 **id** 、 **su** 、 **who** 、 **usermod**   
- 熟悉用户组管理指令： **groupadd** 、 **groupdel** 、 **groupmod**  
- 熟悉用户和组的修改  
- 了解用户和组相关文件： _passwd文件_ 、 _shadow文件_ 、 _group文件_   

#### 【4】文件权限类
- 熟悉文件属性  
- 熟悉文件属性的修改： **chmod** 改变权限、 **chown** 改变所有者、 **charp** 改变所属组

#### 【5】搜索查找类
- 熟悉搜索查找指令： **find** 查找文件或者目录、 **locate** 快速定位文件路径、 **grep** 过滤查找及 **|** 管道符

#### 【6】压缩和解压类
- 熟悉压缩解压指令：  **gzip**/**gunzip** 压缩、 **zip**/**unzip** 压缩、 **tar** 打包

#### 【7】磁盘查看和分区类
- 了解Linux分区原理
- 熟悉查看和分区指令： **du** 查看文件和目录占用的磁盘空间、 **df** 查看磁盘空间使用情况、 **lsblk** 查看设备挂载情况、 **mount**/**umount** 挂载/卸载、 **fdisk** 分区  

#### 【8】进程管理类
- 了解进程的概念
- 熟悉进程管理指令： **ps** 查看当前系统进程状态、 **kill** 终止进程、 **pstree** 查看进程、 **top** 实时监控系统进程状态、 **netstat** 显示网络状态和端口占用信息   

#### 【9】定时任务调度类
- 了解任务调度概念
- 熟悉 **crontab** 定时任务设置

###  VI/VIM编辑器
- 熟悉常用操作

###  网络配置
- 了解NAT网络模式和桥接网络模式  
- 修改IP地址[指定IP]  
- 设置主机名和hosts映射
  
###  系统管理
- 熟悉 **systemctl** 服务管理指令
- 了解服务的运行级别
- 熟悉关机重启命令： **sync** 、 **halt** 、 **poweroff** 、 **reboot** 、 **shutdown** 

### 软件包管理
- 熟悉RPM包的查询、卸载、安装  
- 熟悉YUM的常用命令、修改网络YUM源  

###  shell脚本
#### 【1】hello world！
- 了解shell相关概念
- 了解shell脚本基本流程及执行方式

#### 【2】变量
- 系统预定义变量
- 自定义变量
- 特殊变量

#### 【3】运算符

#### 【4】条件判断

#### 【5】流程控制
- if 判断
- case 语句
- for 循环
- while 循环

#### 【7】read 读取控制台输入

#### 【8】函数
- 系统函数： **basename** 、 **dirname** 
- 自定义函数

## 3、来源参考
[1].  [黑马程序员](https://www.bilibili.com/video/BV1n84y1i7td?p=1&vd_source=ce60d763111e153f4b39f38fc7bfd6c0)  
[2].  [吴光科老师](https://www.bilibili.com/cheese/play/ss703?csource=Hp_searchresult&spm_id_from=333.337.0.0)  
[3].  [韩顺平老师](https://www.bilibili.com/video/BV1Sv411r7vd?p=1&vd_source=ce60d763111e153f4b39f38fc7bfd6c0)  
[4].  [尚硅谷老师](https://www.bilibili.com/video/BV1WY4y1H7d3/?spm_id_from=333.337.search-card.all.click&vd_source=ce60d763111e153f4b39f38fc7bfd6c0)