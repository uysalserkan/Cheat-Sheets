# Docker Cheat Sheet

Docker, uygulamalarınızı container kullanarak hızla derlemenize, test etmenize ve dağıtmanıza imkan tanıyan bir yazılım platformudur. -*Amazon*

- [Docker Cheat Sheet](#docker-cheat-sheet)
  - [Container işlemleri](#container-işlemleri)
    - [Yaşam dögüsü](#yaşam-dögüsü)
    - [Başlatma / Durdurma](#başlatma--durdurma)
    - [Bilgilendirme](#bilgilendirme)
    - [Import / Export](#import--export)
    - [Komut Çalıştırma](#komut-çalıştırma)
  - [Images](#images)
    - [Yaşam Döngüsü](#yaşam-döngüsü)
    - [Imaj Bilgilendirme](#imaj-bilgilendirme)
    - [Örneklendirme](#örneklendirme)
  - [Networks](#networks)
    - [Yaşam Dögüsü](#yaşam-dögüsü-1)
    - [Network Bilgilendirme](#network-bilgilendirme)
    - [Bağlantı](#bağlantı)
  - [Repository](#repository)
  - [Security](#security)
  - [Prune](#prune)

## Container işlemleri

### Yaşam dögüsü

- `docker create`: Bir container oluşturur fakat çalıştırmaz.
- `docker rename`: Container'ların yeniden adlandırmaya yarar.
- `docker run`: Tek bir komut ile Container oluşturur ve çalıştırır.
- `docker rm`: Bir Container siler.
- `docker update`: Container'ın sahip olduğu limitleri günceller.

`docker run -td container_id` komutu ile *container_id*'yi çalıştırırız ve *-t* parametresi ile sanal-TTY başlatır, *-d* ile arkaplanda çalışmaya devam eder.

`docker run --rm` komutu ile çalıştırdığımız zaman, container sonlanması ile birlikte hafızadan kapladığı alan silinecektir.

### Başlatma / Durdurma

- `docker start`: Bir container'ı çalıştırmayı sağlar.
- `docker stop`: Çalışan bir Container'ı durdurmayı sağlar.
- `docker restart`: Çalışan bir Container'ı durdurup tekrar çalıştırmayı sağlar.
- `docker pause`: Çalışmakta olan bir Container'ı *freezing* moduna alır.
- `docker unpause`: *Freezing* modunda olan bir Container'ı tekrar aktif hale getirir.
- `docker wait`: Aktif Container sonlanana kadar o Container'ı engeller.
- `docker kill`: Çalışan bir Container'ı **SIGKILL**'a gönderir.
- `docker attach`: Çalışan bir Container'a bağlanmayı sağlar.

`docker run -it -c 512 container_id` komutu ile işlemcimizin **%50**'sini kullanmasına izin veriyoruz. (*1024 yapmamız halinde %100'ünü kullanacaktır.*)

`docker run -it --cpuset-cpus=0, 4, 6 container_id` komutu ile çalışırken işlemcimizde bulunan hangi çekirdekleri kullanıcağını belirtebiliriz.

`docker run -it -m 300M container_id` komutu ile Container'ın çalışırken kullanacağı maksimum bellek miktarını belileyebiliriz.

`docker run --rm -it --cap-add SYS_ADMIN container_id` komutu ile Container'a sistemimiz üzerinde kullanabileceği belirli yetkiler verebiliriz.

### Bilgilendirme

- `docker ps`: Sistem üzerinde çalışmakta olan Container'ları gösterir.
- `docker logs`: Sistem üzerindeki Container'lar hakkındaki log kayıtlarını gösterir.
- `docker inspect`: Container hakkındaki tüm bilgileri gösterir.
- `docker events`: Container'dan event bilgisini getirir.
- `docker port`: Container'ın kullandığı açık port bilgilerini gösterir.
- `docker top`: Container içerisindeki çalışmakta olan processleri gösterir.
- `docker stats`: Container'ın kullandığı sistem miktar bilgilerini gösterir.
- `docker diff`: Container'daki değişen dosyaları gösterir.

`docker ps -a` komutu ile başlamış ve bitmiş olan Container bilgilerini gösterir.

`docker stats --all` komutu ile tüm Container'ların bilgilerini gösterir.

### Import / Export

`docker cp` komutu ile Container - sistem dosyası arasında dosya/klasör kopyalama işlemi gerçekleştirilir.

`docker export` komutu tüm Container'ı **tarball** olarak sisteme çıkartır.

### Komut Çalıştırma

`docker exec -it foo /bin/bash`, bash üzerinde foo komutunu çalıştırır. Bu mantık dahilinde kendize göre uygulayabilirsiniz.

## Images

### Yaşam Döngüsü

- `docker images`: Docker üzerinde bulunan tüm imajları gösterir.
- `docker import`: *Tarball*'dan bir imaj üretir.
- `docker build`: *Dockerfile* üzerinden bir imaj üretir.
- `docker commit`: Container üzerinden bir imaj üretir ve eğer çalışıyorsa durdurur.
- `docker rmi`: İmajı docker üzerinden siler.
- `docker load`: Bir imaj dosyasını *tar arşivi* içerisinden yükler.
- `docker save`: Bir imaj dosyasını *tar arşivi* olarak dışarıya aktarır.

### Imaj Bilgilendirme

`docker history` komutu ile imaj geçmişini görüntüleyebiliriz.
`docker tag` komutu ile imajın adına bir tag ekleyebiliriz.

### Örneklendirme

`docker load > my_image.tar.gz`

`docker save my_image:tag | gzip > my_image.tar.gz`

`cat my_container.tar.gz | docker import - my_image:tag`

`docker export my_container | gzip > my_container.tar.gz`

## Networks

### Yaşam Dögüsü

- `docker network create my_network`: my_network adında yeni bir network oluşturur.
- `docker network rm my_network`: my_network adındaki network'ü dockerden kaldırır.

### Network Bilgilendirme

- `docker network ls`: Docker üzerinde bulunan networkleri listeler.
- `docker network inspect my_network`: my_network adındaki network'ün içerisini incelememize olanak sağlayan kod.

### Bağlantı

- `docker network connect network_id container_id`: Container belirtilen network'e bağlanır.
- `docker network disconnect network_id container_id`: Container belirtilen network'den ayrılır.

## Repository

- `docker login`: Docker Hub'a giriş işlemini gerçekleştiririz.
- `docker logout`: Docker Hub'dan çıkış yapma işlemini gerçekleştiririz.
- `docker search`: Docker Hub üzerinde bulunan **imajlar**'ı aramamızı sağlar.
- `docker pull`: Docker Hub üzerinden bir **imaj** çekmemizi sağlar.
- `docker push`: Docker Hub'a oluşturduğumuz bir İmaj'ı yüklemeyi gerçekleştirir.

## Security

- `docker run --pids-limit=64`: Docker *1.11*'den sonra aktif hale gelen bir komuttur, Container çalışırken içerisinde çalışacak olan process'lerin maksimum sayısını belirleyebiliyoruz böylece.
- `docker -d --iic=false --iptalbes`: İç processlerin birbiri arasında iletişim kurmasını engeller.
- `docker run --read-only`: Container'ı sadece okuma modunda çalıştırmayı gerçekleştirir.
- `docker run -v $(pwd)/secrets:/secrets:ro debian`: Beliritlen **Volume**'yi sadece okuma modunda Container'a verip çalıştırmaya yarar.

## Prune

- `docker system prune`: Docker sistemini tamamen temizler.
- `docker volume prune`: Docker üzerinde daha önceden tanımlanmış olan tüm Volume bölgelerini kaldırır.
- `docker network prune`: Docker üzerinde bulunan tüm network'leri kaldırır.
- `docker container prune`: Docker üzerinde çalışmış olan tüm Container'ları kaldırır.
- `docker image prune`: Docker üzerinde bulunan tüm imajları siler.

