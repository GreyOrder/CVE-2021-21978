# CVE-2021-21978
CVE-2021-21978 RCE exp

影响版本
VMware View Planner Harness 4.X

与 CVE-2021-21978 类似，该漏洞可以在未授权访问的情况下，上传任意文件，并通过修改自带 py 脚本实现远程代码执行。
值得注意的是，执行命令是在 docker 容器中，并不是直接在系统中执行。

用法：

```
go run CVE-2021-21978.go -h <target ip> -c <cmd>
```

<img src="https://raw.githubusercontent.com/GreyOrder/CVE-2021-21978/main/example.png">
