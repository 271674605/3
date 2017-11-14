1.新建文件夹，将android-a33vr.tar.bz2_* lichee-a33vr.tar.bz2 v3.tar.bz2 lichee-pos.rar pos.tar.bz2拷贝到文件夹下
2.合并文件 cat  android-a33vr.tar.bz2_*> android-a33vr.tar.bz2
  检查压缩包是否有损坏并解压，md5如下：
	5f52d874a5e40eb6bfb246d27928e3b2  lichee-a33vr.tar.bz2
	0495d7561ac9c378d9819d45ef4a5662  android-a33vr.tar.bz2
3.编译内核：
  进入内核： cd lichee
  编译内核： ./build.sh 
4.编译Android
  1)进入android目录：cd androd
  2) source build/envsetup.sh
  3) lunch后选择：astar_chiphd-eng
  4) lunch-xw 后选着xw_pub/pos
  4）extract-bsp
  5）make
  6) pack后生成的固件在lichee/tools/pack/下面