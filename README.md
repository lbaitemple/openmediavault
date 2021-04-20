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

change keys
```
gpg --keyserver  keyserver.ubuntu.com --recv-keys 9165938D90FDDD2E
gpg --export --armor  9165938D90FDDD2E | sudo apt-key add -
```

```
sudo nano /etc/hosts
```
append
```
199.232.68.133 raw.githubusercontent.com
```

```
sudo nano /etc/environment
```

add
```
export http_proxy="http://10.0.0.6:8080"
export https_proxy="http://10.0.0.6:8080"
export no_proxy="localhost, 127.0.0.1"
```

Try to run
```
wget -O - https://github.com/OpenMediaVault-Plugin-Developers/installScript/raw/master/install | sudo bash
```
