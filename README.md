
# [N1盒子] 【20200506重磅更新】N1适配CoreELEC-9.2.2 # 
N1使用的coreELEC-8.90.5已经编译完成，正常情况下写入U盘，插入N1,启动，若要写入emmc，开启ssh，用户名、密码：root、coreelec，登录后执行installtointernal。写U盘启动CoreELEC后，ssh登录系统，执行installtointernal，按屏幕提示操作完成。
# 非自己原创，算是搬运工吧，感谢github的RuralHunter，N1的CoreELEC下载地址https://github.com/RuralHunter/CoreELEC/releases，下载.gz结尾的镜像，写入U盘即可。
 # 写入后只能用U盘，该镜像没有写入emmc脚本，我觉得还是写入比较好，研究了一下，提取了@momokind  https://www.right.com.cn/forum/thread-331363-1-1.html大神的写入脚本，只需把5个文件复制到flash分区即可。大致说下步骤吧！
 * 下载coreelec 9.2.2镜像，解压出img镜像，写入U盘
 * 写入U盘后，电脑会有一个COREELEC命名的盘符，把5个写入文件复制到根目录即可
 * U盘插入N1，开机，此时会进入U盘的系统，设置ssh开启，电脑ssh连接N1，用户名root，密码默认为coreelec，输入/flash/installtoemmc命令，第一个提示输入yes，剩下的全部y，然后N1会重新启动（此时还是U盘系统，但是此步必须做），进入U盘系统后，关机，拔下U盘，开机，OK，大功告成！
