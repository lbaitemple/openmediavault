# openmediavault

```
sudo nano /etc/apt/sources.list
```
add
```
deb http://mirrors.tuna.tsinghua.edu.cn/raspbian/raspbian/ buster main non-free contrib rpi
deb-src http://mirrors.tuna.tsinghua.edu.cn/raspbian/raspbian/ buster main non-free contrib rpi
```

```
sudo nano /etc/apt/sources.list.d/raspi.list
```
add
```
deb http://mirrors.tuna.tsinghua.edu.cn/raspberrypi/ buster main ui
```

Try to run
```
wget -O - https://github.com/OpenMediaVault-Plugin-Developers/installScript/raw/master/install | sudo bash
```
