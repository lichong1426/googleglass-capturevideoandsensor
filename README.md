内部模式主要有两种
1.单纯的传感器数据显示并记录在数据库中
这部分的代码还没有优化，写入的速度为100ms，后期修改为线程会好很多

2.录像的同时记录传感器数据
经过优化还是有稍微卡顿

额外说明：
1.数据库使用SQLite
2.每天一个文件夹，录制的视频和数据库文件文件名相同。目录在DCIM下，sensors目录是模式1，vidoandsensor是模式2
3.谷歌眼镜比较奇葩，要看到新文件需要重启一下眼镜，要不就使用adb pull取出


2018-10-20