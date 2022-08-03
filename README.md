# Kullanım

## Kafka Starter e Giriyoruz

*docker-compose.yml ın içindeki environment in altında yer alan kısımdan Ip adresi ekliyoruz (resimde beyaz çizgiyle belirtilen yer)* ![image](https://user-images.githubusercontent.com/110333072/182684740-23cb17d6-a9cf-43e4-b2e1-dc06ca14df69.png)

## Terminal ' e docker.compose up-d yazınız
![image](https://user-images.githubusercontent.com/110333072/182687016-d2903d04-a073-475b-8a0c-88cecc99dc49.png)


## Debezium ' u çalıştırmak için replicaSet oluşturulması gerekiyor.Bunun için:
**Mongo-Starter** *e giriyoruz. docker-compose.yaml ' ın içindeki ReplicaSet ismini comand : yanındaki deneme yazısını değştirerek değiştirebilirsiniz(resimde beyaz çizgiyle belirtilen yer)*
![image](https://user-images.githubusercontent.com/110333072/182686787-b1786536-6cf9-4c0b-bac3-35bff8382ad9.png)

## Commands.txt 'de de yer alan aşağıdaki komutları sırasıyla yazıyoruz

docker container exec -it mongodb bash
mongo
config = {"_id":"deneme","members":[{"_id":0,"host":"192.168.0.12:27017"}]} 
>_id: -> replica set ismi(resimde gösterilen yere deneme yazısını silerek replica set ismi giriniz
![image](https://user-images.githubusercontent.com/110333072/182687571-66657260-bad8-44f3-a3bf-eb852a79482f.png)






