# MTProxy TLS 绿色版一键安装脚本和t

## 安装

执行如下代码进行安装

```bash
## 新建目录
mkdir /home/mtproxy && cd /home/mtproxy

## 开始安装
curl -s -o mtproxy.sh https://raw.githubusercontent.com/huaniangzi/TGMTProxy-TLS/main/mtproxy.sh && chmod +x mtproxy.sh && bash mtproxy.sh
```

 ![demo.png](https://raw.githubusercontent.com/huaniangzi/TGMTProxy-TLS/main/demo.png)

## 使用

运行服务

```bash
bash mtproxy.sh start
```
调试运行

```bash
bash mtproxy.sh debug
```

停止服务

```bash
bash mtproxy.sh stop
```

重启服务

```bash
bash mtproxy.sh restart
```



## 卸载安装

因为是绿色版卸载极其简单，直接删除所在目录即可。

```bash
rm -rf /home/mtproxy
```

## 开机启动

```bash
chmod 755 /home/mtproxy/mtproxy.sh

vi /etc/crontab

## 加入下面这条命令后保存即可；

cd /home/mtproxy && bash mtproxy.sh start > /dev/null 2>&1 &
```

## 备用项目
[备用项目一、](https://github.com/huaniangzi/TGMTProxy-TLS/blob/main/备用项目.md)
