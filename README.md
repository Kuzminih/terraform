# terraform
terraform notes

# Terraform import
```
При ручном изменение ресурсов в яндекс облаке
Посмотреть к какому реурсу он относиться 
terraform state show
terraform state show 'module.ec2-c.yandex_compute_disk.disks["mongo3-data"]'
terraform state list

terraform import 'module.ec2-c.yandex_compute_disk.disks["mongo3-1-data"]' epd0bjdc8rhda2u4f7s3
module.ec2-c.yandex_compute_disk - к чему относиться 
disks["mongo3-1-data"] что добавить
ID смотреть в облаке
Добавлял я диск mongo3-1-data
Это добавить состояния в фаил state.
Все ADDR можно посмотреть  'terraform state show'
ID в облаке
Если данные есть, но есть изменения в id или в конфигурации ВМ диск не подключен (state show)
Обновляем и проверям
terraform 'refresh/state show'
```
