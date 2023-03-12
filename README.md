

# 安装&升级
```
bash <(curl -Ls https://raw.githubusercontent.com/Jimmy-CHN/x-ui-1/main/install.sh)
```

#ContOS Yum安装wget
```
yum -y install wget     
```

#Debian Ubuntu安装 wget
```
apt-get install wget   
```

#Ubuntu/Debian 系统安装 Curl 方法
```
apt-get update -y && apt-get install curl -y    
```

#Centos 系统安装 Curl 方法
```
yum update -y && yum install curl -y            
```

#使用netstat命令可以快速的查看哪些端口被占用了，包含了TCP端口和UDP端口。
```
netstat -antup   
```

#启动防火墙命令：
```
systemctl start firewalld
```

#关闭防火墙命令：
```
systemctl stop firewalld
```

#重启防火墙命令：
```
firewall-cmd --reload
```

#开放端口命令：
```
firewall-cmd --zone=public --add-port=5011/tcp --permanent
```
命令含义：
–zone #作用域
–add-port=1935/tcp #添加端口，格式为：端口/通讯协议
–permanent #永久生效，没有此参数重启后失效


################################################################################################

#Debian/Ubuntu 命令
```
apt update -y          
```
#Debian/Ubuntu 命令
```
apt install -y curl socat    
```

```
bash <(curl -Ls https://raw.githubusercontent.com/vaxilu/x-ui/master/install.sh) 
```
```
bash <(curl -Ls https://raw.githubusercontent.com/Jimmy-CHN/x-ui-1/blob/main/install.sh)
```

#######################################
完成 X-ui 安装以后，我们可以输入 VPSIP:端口（如1.1.1.1:12345） 登录 X-ui 的管理面板（可以登录代表安装成功） 
# 登入不成功的话，关闭防火墙试试。
########################################

在 VPS 输入 x-ui 命令，进入 X-ui 的命令菜单

申请证书 不要写任何前缀，只需要一级域名即可

申请成功以后，证书和密钥文件在 VPS 目录的 /root/cert 文件夹里面

vless   端口一定要443   传输协议 ws   路径随便  tls打开  域名填解析号的     秘钥复制路径

请求头需要修改 前面添加 host|xxxx

TLS的服务器地址要是完整的域名
