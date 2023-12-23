<h1 align="center">
  <br>
  <a href="https://www.uusec.com">森罗</a>
</h1>

<h4 align="center">来自有安科技的超高速网络空间测绘引擎。</h4>

<p align="center">
<a href="https://github.com/Safe3/senluo/releases"><img src="https://img.shields.io/github/downloads/Safe3/senluo/total">
<a href="https://github.com/Safe3/senluo/graphs/contributors"><img src="https://img.shields.io/github/contributors-anon/Safe3/senluo">
<a href="https://github.com/Safe3/senluo/releases/"><img src="https://img.shields.io/github/release/Safe3/senluo">
<a href="https://github.com/Safe3/senluo/issues"><img src="https://img.shields.io/github/issues-raw/Safe3/senluo">
<a href="https://github.com/Safe3/senluo/discussions"><img src="https://img.shields.io/github/discussions/Safe3/senluo">
</p>
<p align="center">
  <a href="#特色">特色</a> •
  <a href="#使用">使用</a> •
  <a href="#为安全工程师">为安全工程师</a> •
  <a href="#鸣谢">鸣谢</a> •
  <a href="#联系">联系</a> •
  <a href="#授权">授权</a>
</p>


<p align="center">
  <a href="https://github.com/Safe3/senluo/blob/main/README.md">English</a>
  <a href="https://github.com/Safe3/senluo/blob/main/README_CN.md">中文</a>
</p>


---

与NMAP、Shodan和Censys等许多产品一样，Senlo用于网络空间测绘，但其扫描速度比NMAP快10多倍，可以在几分钟内轻松识别数百万端口的网络服务类型。它还具有轻量级、单文件、跨平台和无附加依赖性等特性。



## 特色

<h3 align="center">
  <img src="https://github.com/Safe3/senluo/blob/main/senluo.png" alt="Senluo" width="700px">
  <br>
</h3>
<h3 align="center">
  <img src="https://github.com/Safe3/senluo/blob/main/results.png" alt="Results" width="700px">
  <br>
</h3>

 - 超级快速简单基于探测的**ICMP/TCP/UDP**协议扫描
 - 针对易用性和**资源轻量级**进行了优化
 - 识别常见的网络服务协议和指纹
 - 超大范围网络IP和域名扫描
 - **IPv4/IPv6** 端口扫描
 - 使用crt.sh等进行被动域名枚举
 - **主机发现**扫描
 - 小型、单文件、跨平台且无其他依赖关系
 - 多输入支持 - **HOST/IP/CIDR/FILE**
 - 输出格式支持 - **JSON**



## 使用

```sh
senluo -help
```

这将显示该工具的帮助。以下是它支持的所有选项。


```console
Usage of senluo:
  -Dn
        跳过域枚举发现（默认为true）
  -Pn
        跳过主机ping发现
  -c int
        内部工作线程数（默认10000）
  -h string
        要扫描的主机（逗号分隔）或文件名
  -it int
        超时前等待的空闲毫秒（默认值2000）
  -o string
        要将输出写入的文件（可选）（默认为“target.json”）
  -p string
        要扫描的端口（逗号分隔）[all，top100，top1000,80443100-200]（默认为“top100”）
  -r int
        每秒要发送的数据包（默认为10000）
  -sV
        服务和指纹发现（默认为true）
  -t string
        端口扫描类型[tcp/udp/all]（默认为“all”）
  -tt int
        超时前等待的总毫秒数（默认为60000）
  -v string
        显示详细输出级别（默认为“错误”）
  -version
        显示版本
```

### 运行森罗

扫描目标域名和IP范围。

```sh
senluo -h www.uusec.com,3.3.3.3/24
```



## 为安全工程师

森罗提供了大量功能，有助于安全工程师在其组织中自定义工作流程。通过各种扫描功能（如DNS、HTTP、SMB、DB），安全工程师可以轻松地使用森罗创建他们的自定义检查平台。



## 鸣谢

感谢所有了不起的社区贡献者发送PR，并不断更新这个项目，欢迎给本项目点赞 :heart:

如果你有想法或某种改进，欢迎你贡献并参与该项目，随时发送你的PR。

<p align="center">
<a href="https://github.com/Safe3/senluo/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=Safe3/senluo&max=500">
</a>
</p>

## 联系

<p><span style="unicode-bidi: bidi-override; direction: rtl;">moc.cesuu@troppus</span></p>



## 授权

森罗根据**MIT许可证**进行授权
