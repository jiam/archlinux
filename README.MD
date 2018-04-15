# archbang 安装

设置仓库
````
sudo vi /etc/pacman.d/mirrorlist 
sudo pacman -Syu

````
中文环境配置
````
sudo pacman -S wqy-microhei
sudo pacman -S fcitx
sudo pacman -S fcitx-im
sudo pacman -S fcitx-configtool
````
设置fcitx环境变量
cat >  ~/.config/openbox/environment 
export GTK_IM_MODULE=fcitx
export QT_IM_MODULE=fcitx
export XMODIFIERS="@im=fcitx"
````

配置fcitx自启动
````
echo "/usr/bin/fcitx-autostart" >> ~/.config/openbox/autostart 
````
