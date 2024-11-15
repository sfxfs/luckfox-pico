# 在 WSL Ubuntu 24 中编译遇到的问题

请全程保证能访问外网（TUN 模式）

## python 没有指向 python3 导致报错没有这个命令

```shell
sudo apt install python-is-python3
```

## PATH 包含 \n

把 PATH 覆盖掉为这个：`/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`

或者换成虚拟机编译即可

## cpio 没找到

```shell
sudo apt install cpio
```

