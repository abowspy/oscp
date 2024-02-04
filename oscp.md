#### <font color="#7030a0">SSH</font>
```shell
chmod 600 id_rsa
ssh -i id_rsa root@10.10.10.10
```
#### <font color="#7030a0">遠端桌面</font>
```shell
xfreerdp /cert-ignore /size:87% /v:10.10.10.10 /u:username /p:password
```
#### <font color="#7030a0">Telnet</font>
```shell
telnet 10.10.10.10
```
##### <font color="#7030a0">安裝telnet</font>
```shell
dism /online /Enable-Feature /FeatureName:TelnetClient
```
##### <font color="#7030a0">Terminal切換模式</font>
快捷鍵 `Ctrl + p`
```shell
┌──(kali㉿kali)-[~]
└─$ 

kali@kali:~$
```
##### <font color="#7030a0">發送mail</font>
```shell
sudo swaks -t rc@xx.com --from send@xx.com --attach @config.Library-ms --server 10.10.10.10 --body "read me" --header "Subject: title" --suppress-data -ap
```
