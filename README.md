<h1 align="center">
  <br>
  <a href="https://www.uusec.com">Senluo</a>
</h1>

<h4 align="center">Super fast cyberspace scanner based on uusec technology.</h4>

<p align="center">
<a href="https://github.com/Safe3/senluo/releases"><img src="https://img.shields.io/github/downloads/Safe3/senluo/total">
<a href="https://github.com/Safe3/senluo/graphs/contributors"><img src="https://img.shields.io/github/contributors-anon/Safe3/senluo">
<a href="https://github.com/Safe3/senluo/releases/"><img src="https://img.shields.io/github/release/Safe3/senluo">
<a href="https://github.com/Safe3/senluo/issues"><img src="https://img.shields.io/github/issues-raw/Safe3/senluo">
<a href="https://github.com/Safe3/senluo/discussions"><img src="https://img.shields.io/github/discussions/Safe3/senluo">
</p>
<p align="center">
  <a href="#features">Features</a> •
  <a href="#usage">Usage</a> •
  <a href="#for-security-engineers">For Security Engineers</a> •
  <a href="#credits">Credits</a> •
  <a href="#contact">Contact</a> •
  <a href="#license">License</a>
</p>


<p align="center">
  <a href="https://github.com/Safe3/senluo/blob/main/README.md">English</a> •
  <a href="https://github.com/Safe3/senluo/blob/main/README_CN.md">中文</a>
</p>


---

Senluo is used for cyberspace surveying and mapping, just like many products such as NMAP, Shodan, and Centsys, but its scanning speed is more than 10 times faster than NMAP, making it easy to identify network service types with millions of ports in minutes. It also has features such as lightweight, single file, cross platform, and no additional dependencies.

## Features

<h3 align="center">
  <img src="https://github.com/Safe3/senluo/blob/main/senluo.png" alt="Senluo" width="700px">
  <br>
</h3>
<h3 align="center">
  <img src="https://github.com/Safe3/senluo/blob/main/results.png" alt="Results" width="700px">
  <br>
</h3>

 - Super fast and simple **TCP/UDP** probe based scanning
 - Optimized for ease of use and **lightweight** on resources
 - Identify common network service protocols and fingerprints
 - Ultra wide range network IP and domain name scanning
 - **IPv4/IPv6** Port scan 
 - **Passive** domain enumeration using crt.sh,etc
 - **Host Discovery** scan
 - Small, single file, cross platform, and no additional dependencies
 - Multiple input support - **HOST/IP/CIDR**
 - Output format support - **JSON**

## Usage

```sh
senluo -help
```

This will display help for the tool. Here are all the switches it supports.


```console
Usage of ./senluo:
  -Dn
    	Skip domain enumerate discovery (default true)
  -Pn
    	Skip host ping discovery
  -c int
    	general internal worker threads (default 10000)
  -h string
    	hosts to scan for (comma-separated)
  -o string
    	file to write output to (optional)
  -p string
    	ports to scan (comma-separated)[all,top100,top1000,80,443,100-200] (default "top100")
  -r int
    	packets to send per second (default 10000)
  -sV
    	Service discovery
  -t string
    	type of port scan [tcp/udp/all] (default "all")
  -timeout int
    	millisecond to wait before timing out (default 2000)
  -v string
    	display verbose output level (default "error")
  -version
    	display version
```

### Running Senluo

Scanning target domain and IPs.

```sh
senluo -h www.uusec.com,3.3.3.3/24
```


## For Security Engineers

Senluo offers great number of features that are helpful for security engineers to customise workflow in their organization. With the varieties of scan capabilities (like DNS, HTTP, SMB, DB), security engineers can easily create their suite of custom checks with Senluo.


## Credits

Thanks to all the amazing [community contributors for sending PRs](https://github.com/Safe3/senluo/graphs/contributors) and keeping this project updated. :heart:

If you have an idea or some kind of improvement, you are welcome to contribute and participate in the Project, feel free to send your PR.

<p align="center">
<a href="https://github.com/Safe3/senluo/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=Safe3/senluo&max=500">
</a>
</p>

## Contact

<p><span style="unicode-bidi: bidi-override; direction: rtl;">moc.cesuu@troppus</span></p>



## License

Senluo is distributed under [**MIT License**]
