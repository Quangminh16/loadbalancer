Hệ thống cân bằng tải gồm 3 ubuntu server 20.04. Trong mỗi ubuntu server ta cài 3 phần mềm là Apache, Haproxy, Keepalived.
địa chỉ ip : server1: 192.168.2.123; server2: 192.168.2.124; server3: 192.168.2.125. Và 3 server này có chung địa chỉ ip ảo là: 192.168.2.100
hệ thống hoạt động như sau: request được gửi đến ip: 192.168.2.100 sau đó keepalived sẽ chuyển yêu cầu đến haproxy và haproxy sẽ làm nhiệm vụ cân vằng tải rồi gửi resquest đến webserver
