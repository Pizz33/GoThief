# GoThief
集成了截图 键盘记录 剪贴版功能，用于网络限制场景下的信息搜集

## 背景
最近在攻防比赛中碰到这样的场景，目标机器访问内部应用系统由VPN进行统一管控，连接VPN后会断开与外网的连接，导致不能实时下发指令

因此便有了这个小工具的想法，通过截图 键盘记录 剪贴版获取目标在连接VPN后的操作，搜集敏感信息进行下一步的横向

## Usage

通过输入不同参数调用不同功能，默认输出文件保存至目录 `C:\Users\Public\Gothief` 
```
go build -trimpath -ldflags="-s -w -H windowsgui" main.go

  -c    clipboard 剪贴板
  -k    keylogger 键盘记录
  -s    screenshots 截屏
```
## 实现效果

![image](https://github.com/Pizz33/GoThief/assets/88339946/6d7282e9-640c-4253-b63e-38ed46ed35ce)

![image](https://github.com/Pizz33/GoThief/assets/88339946/eeff920c-78a7-4c96-ac66-22bcd6be8876)
