# USB-Redirector
USB Redirector(USB共享工具)

 USB Redirector官方版是一款功能强大的USB共享工具。USB Redirector最新版支持多种USB设备，无需安装驱动即可共享，支持本地和远程USB设备管理，支持Windows和Linux系统间USB设备共享，网络连接断开时自动尝试重连，助您轻松实现USB共享。

      1、排除清单：阻止特定设备被共享或连接。

      2、IP过滤：控制访问USB服务器的计算机。

      3、超时释放：自动释放长时间未使用的设备。

      4、多设备共享：选择性地共享多个相同设备。

      5、流量压缩：优化网络流量，提升USB设备操作效率。

      6、访问控制：通过ACL功能，仅允许特定计算机使用USB设备。

      7、自动共享：USB设备插入时自动共享，简化操作。

      8、NAT穿透：支持NAT网络中的USB设备连接。

      9、自定义命名：为相同设备分配独特名称，便于区分。

      10、设备策略：通过规则控制USB设备的共享和连接。



      1、虚拟机访问：轻松访问Hyper-V等虚拟机中的USB设备。

      2、USB服务器组织：为公司或家庭网络中的用户提供功能齐全的USB服务。

      3、USB端口问题：解决USB端口损坏或丢失的计算机上的USB设备使用问题。

      4、跨平台重定向：支持Windows和Linux之间的USB设备重定向。

      5、物理访问限制：限制对USB设备的物理访问，但保持网络访问。

软件特点

      1、跨平台支持：支持Windows和Linux系统间USB设备共享。

      2、空闲设备再利用：允许重新连接未使用的USB设备。

      3、NAT穿透：即使在网络路由器后也能共享USB设备。

      4、一体化设计：USB服务器和客户端功能集成，简化操作。

      5、高速共享：支持高速USB设备如网络摄像机和音频设备。

      6、无驱共享：无需安装驱动即可共享USB设备。

      7、黑名单功能：阻止特定计算机访问USB设备。

      8、自动连接：远程USB设备自动连接。

      9、远程控制：远程管理USB设备。

      10、自动重连：网络连接断开时自动尝试重连。

      11、排除清单：灵活控制共享的USB设备。

```
      查询BUSID：usbipd list
      查询主机的IP地址：ipconfig
      分享USB设备：usbipd bind --busid=<BUSID>
      解除分享USB设备的代码：usbipd unbind --busid=<BUSID>


      apt install linux-tools-virtual hwdata
      update-alternatives --install /usr/local/bin/usbip usbip `ls /usr/lib/linux-tools/*/usbip | tail -n1` 20
      使用usbip help测试是否安装成功

      使用usbip连接主机分享的USB设备
      usbip attach --remote=<HOST_IP> --busid=<HOST_BUSID>
```
