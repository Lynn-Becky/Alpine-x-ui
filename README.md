注意！由于F大x-ui已经停止更新，目前面板不适配部分新版的xray内核的内容，本项目即日起归档。同时为了面板安全，若仍然使用请激活tls以保证安全，[3x-ui](https://github.com/MHSanaei/3x-ui)已经支持在Alpine linux安装，建议使用。
# x-ui
适配Alpine linux  使用F大编译的x-ui，支持reality协议  
默认端口9000，可使用x-ui命令更换  
ovz，lxc虚拟化的vps，在纯净系统首次安装后内存占用约为27m左右，重启后内存占用约为20m

# 功能介绍

- 系统状态监控
- 支持多用户多协议，网页可视化操作
- 支持的协议：vmess、vless、trojan、shadowsocks、dokodemo-door、socks、http
- 支持reality的配置
- 支持配置更多传输配置
- 流量统计，限制流量，限制到期时间
- 可自定义 xray 配置模板
- 支持 https 访问面板（自备域名 + ssl 证书）
- 更多高级配置项，详见面板

# 安装&升级

```
apk add curl&&apk add bash && bash <(curl -Ls https://raw.githubusercontent.com/Lynn-Becky/Alpine-x-ui/main/alpine-xui.sh)
```
仅支持Alpine linux 安装  
支持x86与arm64架构的小鸡安装
# 部分问题解决方案
若跑太猛，面板crashed了，请使用以下命令重启面板
```
/etc/init.d/x-ui restart
```
特别感谢mocikate大佬，安装脚本有部分参考其脚本并修改  
感谢F大编译维护的x-ui
