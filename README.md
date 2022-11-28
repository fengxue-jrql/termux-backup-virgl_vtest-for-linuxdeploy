# termux-backup-virgl_vtest-for-linuxdeploy
termux zink +virgl_vtest for linux deploy kali
download:
微云文件分享:termux-backup-virgl_vtest-for-linuxdeploy.tar.gz下载地址:https://share.weiyun.com/DCdD3ydo文件大小:306.2M

in termux

termux-setup-storage

termux-restore /sdcard/termux-backup-virgl_vtest-for-linuxdeploy.tar.gz

su

MESA_NO_ERROR=1 MESA_GL_VERSION_OVERRIDE=4.0 GALLIUM_DRIVER=zink ZINK_DESCRIPTORST=auto  /data/data/com.termux/files/usr/bin/virgl_test_server --use-egl-surfaceless

in linux deploy kali


GALLIUM_DRIVER=virpipe MESA_GL_VERSION_OVERRIDE=4.0 yourapp
