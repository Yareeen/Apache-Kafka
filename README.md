# Apache-Kafka
Apache Kafka ile mesajlaşma uygulaması tasarlama

## Giriş
Kafka'yı bir mesajlaşma sistemi olarak kullanarak verileri bir mongodb veritabanına ekliyoruz. Bir tane Üretici (Producer) bulunmaktadır. Her 10 saniyede bir mongodb'de yeni kayıtların olup olmadığını kontrol eder. Eğer veritabanında yeni bir kayıt varsa, bu kaydı bir mesaj olarak Kafka'ya gönderir.
Ayrıca 3 adet Tüketici (Consumer) bulunmaktadır. Kafka'yı dinleyerek herhangi bir mesaj olduğunda bu mesajı konsola yazdırırlar.
Bu uygulamanın ayrıca yeni bir kayıt eklemek için yardımcı bir uygulaması bulunmaktadır. 

### Gereksinimler
Projeyi çalıştırmak için aşağıdaki gereksinimlere ihtiyacınız olacaktır:
- Docker
- Docker Compose
- MangoDB

### Kullanım
- Komut satırına "cd Apache-Kafka" yazılır.
- "docker-compose up" komutuyla docker imageleri oluşturulur. 