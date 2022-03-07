![](https://super-zero-blog.oss-cn-beijing.aliyuncs.com/20220307212240.webp)

## 记录一次我组装的黑苹果主机

[[[https://github.com/Drk-np/msi-z390-.git\]\][https://github.com/Drk-np/msi-z390-.git\]]: 



想学习如何配置黑苹果EFI [请点击这里](https://apple.sqlsec.com "请点击这里")

这也是国光编写的教程，不要问我为什么都跟国光有关系，因为我是国光的小粉丝

### 我的主机配置

|   组件   |          型号          |
| :------: | :--------------------: |
|   CPU    |         9700K          |
|   主板   |    MSI Z390 暗黑版     |
|   内存   |      8G  3000 X 4      |
|   显卡   |       RX560D 4G        |
|   硬盘   | SN750  500G /三星PM981 |
| **网卡** | BCM94360CD 4 天线版本  |

目前黑苹果完成度大概90%以上，其实我已经稳定用了一年了！！！ 稳定性可以

## BIOS设置

- **禁用**

  - Fast Boot
  - Secure Boot
  - Serial/COM Port
  - Parallel Port
  - VT-d (如果设置了 `DisableIoMapper` 为 YES，则可以打开这个选项)
  - CSM
  - Thunderbolt (建议关闭雷电，第一次安装可能出现玄学问题)
  - Intel SGX
  - Intel Platform Trust
  - CFG Lock

  **开启**

  - VT-x
  - Above 4G decoding
  - Hyper-Threading
  - Execute Disable Bit
  - EHCI/XHCI Hand-off
  - OS type: Windows 8.1/10 UEFI Mode
  - DVMT Pre-Allocated(iGPU Memory): 64MB
  - SATA Mode: AHCI

主板设置可以百度 很简单

## 当前OC版本 0.7.8 系统版本是12.3 Beta版

![image-20220307214035311](https://super-zero-blog.oss-cn-beijing.aliyuncs.com/20220307214035.png)

## CPU变频正常 核显现在是辅助计算模式

![image-20220307214206981](https://super-zero-blog.oss-cn-beijing.aliyuncs.com/20220307214207.png)

## Geekbench5 CPU 单核跑分：1137，多核跑分：6703 分

![image-20220307214602686](https://super-zero-blog.oss-cn-beijing.aliyuncs.com/20220307214602.png)

## Geekbench5 显卡OpenCL跑分：14438 分

![image-20220307214821686](https://super-zero-blog.oss-cn-beijing.aliyuncs.com/20220307214821.png)

## USB

USB 定制过：

![image-20220307215029543](https://super-zero-blog.oss-cn-beijing.aliyuncs.com/20220307215029.png)

## 声卡

ALC1220A 声卡，AppleALC 原生支持，注入 layout-id 为 11 即可正常驱动：

![image-20220307215150783](https://super-zero-blog.oss-cn-beijing.aliyuncs.com/20220307215150.png)

## 有线网卡已驱动

![image-20220307215258844](https://super-zero-blog.oss-cn-beijing.aliyuncs.com/20220307215258.png)

## 无线网卡已驱动 毕竟是免驱网卡

![image-20220307215401802](https://super-zero-blog.oss-cn-beijing.aliyuncs.com/20220307215401.png)

随航和通用控制可用，这个功能很香。

![image-20220307215424763](https://super-zero-blog.oss-cn-beijing.aliyuncs.com/20220307215424.png)

## 蓝牙正常

![image-20220307215552179](https://super-zero-blog.oss-cn-beijing.aliyuncs.com/20220307215552.png)

## 隔空投送正常

![image-20220307223050886](https://super-zero-blog.oss-cn-beijing.aliyuncs.com/20220307223050.png)

## 基本上也就这样子了 祝你们Hackintosh成功

