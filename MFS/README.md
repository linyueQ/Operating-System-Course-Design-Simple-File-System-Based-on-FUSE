注意！！！：

	我的磁盘文件的路径写的是绝对路径，所以在使用的时候，一定要在两个C文件的磁盘路径那里更改：
	1. init_disk.c 第75行，"/home/linyueq/homework/MFS/diskimg" 改为您的电脑的磁盘文件的路径
	2. MFS.c 第51行，"/home/linyueq/homework/MFS/diskimg" 改为您的电脑的磁盘文件的路径
	
	文件系统使用步骤：
	① ./init_disk.c
	② ./MFS.c -d fuse
	③ 另开一个终端，进入到目录下面执行各种文件操作即可
	
	PS：这里的fuse是挂载点的名字，用户可以自己创建一个文件夹，然后填写该文件夹的路径以取代fuse
