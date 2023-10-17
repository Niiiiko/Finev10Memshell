# Finev10Memshell
针对finereportv10反序列化接口/webroot/decision/remote/design/channel进行无回显检测并提供Godzilla memshell注入功能（部分环境缺少依赖无法成功）。

因为添加了两个FineReport原生的jar包文件，因此打包后的工具体积较大，经历、水平有限暂不知道怎么解决，如有建议尽管提。

对工具不放心使用的可自行反编译检查。

## 使用方式

无回显命令执行：

```
java -jar FineV10Memshell.jar -u url -c 'command'
```
<img width="949" alt="image" src="https://github.com/Niiiiko/Finev10Memshell/assets/88720946/39e52978-7ac3-4403-8435-4ebbfe72ecfe">
Godzilla memshell注入：

```
java -jar FineV10Memshell.jar -u url -m
```

<img width="948" alt="image" src="https://github.com/Niiiiko/Finev10Memshell/assets/88720946/84257880-25c6-4c08-89dc-f655ff4e740d">
<img width="315" alt="image" src="https://github.com/Niiiiko/Finev10Memshell/assets/88720946/fe1a82e7-c21f-42e8-a808-e3c512364c73">

## 影响

2022-08-12 之前的 FineReport10.0/11.0、FineBI5.1 系列均受影響，非2023利用方式。

## 参考

https://github.com/Avento/FineReport_channel_Deserialization_Vulnerabilities_RCE
