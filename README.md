若Cloudflare的SSL设置为完全，则服务器命令为：
```
./xtunnel -l wss://:443
```
若Cloudflare的SSL设置为灵活，则服务器命令为：
```
./xtunnel -l ws://80
```
若服务器非以上端口，则Cloudflare回源规则要重写端口。

客户端命令：
```
./xtunnel -l socks5://:1080 -f wss://xtunnel.dynv6.net -ip 162.159.38.255
```
