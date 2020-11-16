# Nttcp 网络性能测试工具
nttcp用来测量TCP，UDP和多播UDP连接的传输速率。

# nttcp 工具安装
 
 下载：https://gallery.technet.microsoft.com/NTttcp-Version-528-Now-f8b12769

# 测试方法

   # TCP 测试：

      接收方：ntttcp -r -p 80 -a 6 -t 60 -cd 5 -wu 5 -v -xml c:\bench.xml  -m 1,0,10.10.10.12 1,1,10.10.10.12

      发送方：ntttcp -s -p 80 -a -t 60 -cd 5 -wu 5 -m 1,0,10.10.10.12 1,1,10.10.10.12


   # UDP 测试：

      接收方：ntttcp –r –u -p 80 –t 60 –cd 5 –wu 5 –v –xml c:\bench.xml -m 1,0,10.10.10.12 1,1,10.10.10.12

      发送方：ntttcp -s –u -p 80 -t 60 -cd 5 -wu 5 -m 1,0,10.10.10.12 1,1,10.10.10.12
      
# 参考资料

  http://benjr.tw/94564
  https://aws.amazon.com/cn/premiumsupport/knowledge-center/network-throughput-benchmark-windows-ec2/?nc1=h_ls

