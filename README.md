# iptv_channel_scanner_linux
原理：  
构造igmp包，然后使用libpcap抓包，获取组播地址和端口。  
to compile it:  
		g++ -g -o iptvscanner iptvscanner.cpp -lpcap  
usage: 
	./iptvscanner 239.3.1.1 239.3.1.254  
todo:  
	save m3u playlist  
  
if you don't scan any channel,try to increase timeout by changeing usleep(150000) to sleep(1) or sleep(2)
