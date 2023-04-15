# DHCP
## Домашнее задание по теме _DHCP, PXE_  
> Следуя шагам из документа https://docs.centos.org/en-US/8-docs/advanced-install/assembly_preparing-for-a-network-install
установить и настроить загрузку по сети для дистрибутива CentOS8.  
В качестве шаблона воспользуйтесь репозиторием https://github.com/nixuser/virtlab/tree/main/centos_pxe.  
Поменять установку из репозитория NFS на установку из репозитория HTTP.  
Настроить автоматическую установку для созданного kickstart файла (*) Файл загружается по HTTP.  
Задание со звездочкой *  
автоматизировать процесс установки Cobbler cледуя шагам из документа https://cobbler.github.io/quickstart/.  
Формат сдачи ДЗ - vagrant + ansible  

### Решение ДЗ.  
Задание сделано согласно методичке, но _Ansible_ выполняется через роли.  
После развертывания машины _pxeserver_ запускаем _pxeclient_ из _VirtualBox_  и попадаем на экран выбора установки системы.  

![](https://github.com/Vitaliy7/DHCP/blob/main/screenshots/1.png?raw=true)

После, для автоматизации установки был добавлен _kickstart file_ и теперь меню выбора установки системы выглядит так:  

![](https://github.com/Vitaliy7/DHCP/blob/main/screenshots/2.png?raw=true)
