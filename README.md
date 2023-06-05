# MendeleevaAK_infra
MendeleevaAK Infra repository

Дз №3 Стр 35
1. ssh -i ~/.ssh/appuser -J appuser@51.250.97.102 appuser@10.129.0.22

2. touch ~/.ssh/config
Далее в конфиге прописываем
Host someinternalhost
    HostName 10.129.0.22
    User appuser
    IdentityFIle ~/.ssh/appuser
    ProxyJump appuser@51.250.97.102
Далее подключаемся к someinternalhost командой 
ssh someinternalhost


bastion_IP = 51.250.97.102
someinternalhost_IP = 10.129.0.22


