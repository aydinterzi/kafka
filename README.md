# Basit Kafka Uygulaması(KafkaJS)

## Kafka Nedir?
Apache Kafka LinkedIn tarafından geliştirilen ve şuan Apache bünyesinde bulunan, büyük verileri anlık olarak depolamak ve analiz etmek için kullanılan açık kaynak bir framework’dür. Büyük verileri hızlı bir şekilde depolayıp analiz etmek için ise mesajlaşma sistemini (queue) kullanmaktadır.
## Ne Amaçla Kullanılır?
Gerçek zamanlı veri akışı ve analizi şirketlerin veya kuruluşların anlık olarak gelen güncel bilgiler ile ne stoklamaları neleri satmaları gibi kararları vermesinde yardımcı olur. Şirketler ise karar vermelerini sağlayan bu verileri amaçları doğrultusunda depolayıp analiz etmek için oldukça performanslı olan Apache Kafka’yı kullanırlar. Ne işe yaradığı konusunda kafanızda soru işaretleri kaldıysa daha açıklayıcı bir örnek ile belki bunu giderebiliriz. Popüler ve anlık olarak çok fazla aktif kullanıcıya sahip bir web sitesi, aktif kullanıcıların site içerisindeki davranışlarından haberdar olmak istiyor, düşünüldüğünde binlerce kullanıcının aynı anda bu sitede aktif olarak bir sürü işlem gerçekleştirdiğini sayfadan sayfaya ilerlediğini ve butonlara bastığını varsayalım ve bu verinin toplanması gerektiğini. Oluşan verinin ne kadar hızlı arttığını hayal edin. İşte bu gibi durumlarda şirketler Apache Kafka ve kullandığı mesajlaşma sistemi sayesinde bu kullanıcı loglarını anlık olarak hızlı bir şekilde depolayabilir ve analiz edebilir. Amazon,Netflix, Spotify gibi şirketler bu teknolojiyi aktif olarak kullanmaktadır.
![kafka](https://miro.medium.com/max/1200/1*xj4va4KzjiJGu7baGltJ8g.jpeg)
## Kurulum
### Uygulamayı çalıştırmak için ilk önce zookeeper ve kafka'nın bilgisayarda kurulu olması gerekiyor. 
### Bu kurulumlarla uğraşmamak için *docker-compose.yml* dosyasında gerekli ayarlar yapıldı.
 - ```docker-compose up```komutu ile yml dosyasındaki imagelari sistemimize yüklüyoruz.
 - ```node producer.js ``` ile mesaj üretiyoruz.
 - ```node consumer.js``` ile ürettiğimiz mesajları tüketiyoruz.


## Kaynaklar
### [Kafka Nedir?](https://medium.com/kodcular/kafka-nedir-nas%C4%B1l-%C3%A7al%C4%B1%C5%9Ft%C4%B1r%C4%B1l%C4%B1r-%C3%B6rnek-apache-kafka-react-js-node-js-socket-io-uygulamas%C4%B1-e8ad71e00574)
### [kafkajs](https://kafka.js.org/docs/running-kafka-in-development)