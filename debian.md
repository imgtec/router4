## 使用iphone usb连接上网 ##

```
ipheth-utils
libimobiledevice-dev
libimobiledevice-utils

idevicepair unpair && idevicepair pair
点击信任
```

## 使用菊花3G上网 ##

```
sg_raw /dev/sr0 11 06 20 00 00 00 00 00 01 00
```


## 内网转换 ##

```
WAN0='enp0s20u1u4'
iptables -F
iptables -P INPUT ACCEPT
iptables -P FORWARD ACCEPT
iptables -t nat -A POSTROUTING -o ${WAN0} -j MASQUERADE
```

## 配置dhcp服务器 ##
```
subnet 192.168.42.0 netmask 255.255.255.0 {
  interface enp3s0;
}
```


## 保存转发规则 ##

```
iptables-persistent
/etc/iptables/rules.v4
```

## 配置企业局域网 ##
```
扩展名更改为local.conf
```

## 静态路由表 ##

```
?ifupdown-extra
?/etc/network/routes
```





