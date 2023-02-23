## ssh配置config

Host 35.220.222.252 \
HostName 35.220.222.252 \
ProxyCommand nc -X 5 -x 127.0.0.1:10010 %h %p \
Port 22 \
User oker \
IdentityFile ~/.ssh/id_rsa \
