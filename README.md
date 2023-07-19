#  什么是 WARP？

由 Cloudflare 公司出品的一款改善网络的软件，目的是让你的网络使用更加安全。

官方网址 `https://1.1.1.1/`

官方客户端包括：`Windows`，`MacOS`，`iOS`，`Android`和`Linux`

![WX20230714-142303@2x](https://github.com/SeverideLo/WARP-/assets/83275041/4b2a3f21-98a9-4e47-b88e-dc5c5e94816d)

***

速度测试如下：
```
软件：WARP 官方客户端
网络：Wi-Fi
测试平台：MacOS Ventura 13.2.1，Edge浏览器
视频质量：4K 60FPS HDR
https://youtu.be/mkggXE5e2yk
```
![WX20230714-145244@2x](https://github.com/SeverideLo/WARP-/assets/83275041/9fa70d1f-8f6f-4423-9bf7-ea0ecb830071)

```
软件：WARP 官方客户端
网络：Wi-Fi
测试平台：iPhone 6s Plus ，iOS 15.7，YouTube 客户端
视频质量：1080P 60FPS
https://youtu.be/mkggXE5e2yk
```
![IMG_0006](https://github.com/SeverideLo/WARP-/assets/83275041/fe9c3e98-b961-4e32-80e9-c29f1f9333ee)

```
软件：WARP 官方 Android 客户端
网络：5G 中国联通
测试平台：vivo X80 Pro天玑9000版，Edge 浏览器
视频质量：1080P 60FPS
https://youtu.be/mkggXE5e2yk
```
![WechatIMG1652](https://github.com/SeverideLo/WARP-/assets/83275041/9344afcd-8caa-404b-b454-8c6ab0a89d13)

##  WARP 小总结

一款还不错的，可以看到外面世界的软件，只是默认是全局，导致部分国内的软件会有较高的延迟和检测使用代理的情况，同时流量较少，新用户免费流量仅有 1GB。
同时，WARP 官方安卓客户端，默认是不支持 YouTube 和 Google Photo 客户端的，什么鬼！

#  怎么获取更多流量

软件本身自带的  private-key 只有 1GB 流量，想要获得更多流量，只能通过更换 private-key。

##  方法一

找到 Telegram 机器人 `@generatewarpplusbot`，激活后它会让你关注两个频道

![WX20230719-154811@2x](https://github.com/SeverideLo/WARP-/assets/83275041/9bb5dd47-5c47-45ee-8b68-f74f502b1b94)

都关注后，点击下方的 `I have subscribeed` 即可通过验证。

通过验证后，输入 `/generate` 获取密钥。

这时候机器人会弹出一个人机验证的简单算术题目。

![WX20230719-155154](https://github.com/SeverideLo/WARP-/assets/83275041/98046f9b-1ef3-457b-81dd-effc2d0ce2a9)

这时候根据提示，计算，然后回复答案 `/generate XX`即刻获取 **24PB流量** 的 private-key。同时附带一份 `wg-config.conf` 的文件（后续再说）。

***

##  **注意⚠️**

>每24小时只能获取一枚 private-key，想再要新的 key 只能等待 24小时后再次申请。

>再次申请 private-key 并不会导致以前申请的 key 失效。

>每个 private-key 只能搭载 5 台设备。

***

###  方法二

通过Replit平台生成。

[一键生成24PB流量key](https://replit.com/@ygkkkk/WarpKey-Register-PRO) via`yonggekkk`

打开点击右上角的`Run`即可。

![WX20230719-160810@2x](https://github.com/SeverideLo/WARP-/assets/83275041/ff29e151-7e43-4fe2-90aa-b812d028f10b)

运行一段时间，就能得到内含 24PB 的 private-key。

![WX20230719-160755@2x](https://github.com/SeverideLo/WARP-/assets/83275041/20f582be-167c-4605-a8ec-518541135152)

拿到 24PB 的 private-key 后，再软件里面更换即可。

![WX20230719-161553](https://github.com/SeverideLo/WARP-/assets/83275041/d30edf85-a59b-4625-9550-702c371515f6)

其他系统不演示了，自行学习。

#  进阶使用

因为 WARP 客户端走的是全局代理，开启时会导致绝大部分国内软件用不了或者响应慢，甚至检测出网络异常。

通过上面获取的`private-key`获取附带的`wg-config.conf`文件可以才想到，WARP 其实用的`WireGurad`协议。

So，如果我们用其他支持`WireGuard`协议的代理软件，就能做到分流的效果。

## 实操

