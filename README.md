- Clone kafka-consumer
- Download Kafka di website resmi Apache (pilih yang recommended)
- Ekstrak, buka direktori zookeeper.properties > ubah dataDir untuk jangan diletakkan di tmp/temporary agar settingan tidak hilang setelah restart
- Setting hal yang sama pada server.properties
- Start zookeeper terlebih dahulu:
- Linux: ./bin/zookeeper-server-start.sh config/zookeeper.properties
- Windows: .\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties
- Lalu start kafka:
- Linux: ./bin/kafka-server-start.sh config/server.properties
- Windows: .\bin\windows\kafka-server-start.bat .\config\server.properties
- Abaikan log merah. Jika consumer sudah mendapatkan message broadcast dari producer, berarti sudah berhasil