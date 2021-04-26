# Markdown Cheat Sheet

Giriş seviyesinde bir dosyadır, eğer daha gelişmiş bir halini istiyorsanız iletişime geçebilirsiniz.

- [Markdown Cheat Sheet](#markdown-cheat-sheet)
  - [Dosya Operatörleri](#dosya-operatörleri)
  - [Test Operasyonu](#test-operasyonu)
    - [If-Elif-Else](#if-elif-else)
    - [Switch-Case](#switch-case)
  - [Argümanlar](#argümanlar)
  - [Genel Yapılar](#genel-yapılar)
    - [Satır satır dosya okuma](#satır-satır-dosya-okuma)
    - [Dosyadan belirtileni arama](#dosyadan-belirtileni-arama)
    - [Komut çalıştırma](#komut-çalıştırma)
    - [Değişken tanımlama](#değişken-tanımlama)
    - [Fonksiyon tanımlama](#fonksiyon-tanımlama)
  - [Dosya İşlemleri](#dosya-i̇şlemleri)
  - [Genel Kullanılan Komutlar](#genel-kullanılan-komutlar)


## Dosya Operatörleri

| Operatör          | Açıklaması                                                                         |
| ----------------- | ---------------------------------------------------------------------------------- |
| `> dosya`         | Dosyaya belirtilen şeyleri ekler, eğer dosya bulunmuyorsa dosyayı oluşturup ekler. |
| `>> dosya`        | Dosyanın devamına belirtilen şeyleri ekler.                                        |
| `< dosya`         | Dosyadan okuma yapar.                                                              |
| `dosya1 | dosya2` | Dosya 1'i, Dosya 2 ye ekler.                                                       |

## Test Operasyonu

Köşeli parantezlerin içerisine özel tanımlar yapılabilir, bunlar şöyledir.

| Operatör                | Açıklaması                                                     |
| ----------------------- | -------------------------------------------------------------- |
| `!EXPRESSION`           | Expression tanımlaması yanlış.                                 |
| `-n STRING`             | Belirtilen STRING'in boyutu 0'dan fazladır.                    |
| `-z STRING`             | Belirtilen STRING'in boyutu 0'dır.                             |
| `STRING1 = STRING2`     | STRING1, STRING2'ye eşittir.                                   |
| `STRING1 != STRING2`    | STRING1 STRING2'ye eşit değildir.                              |
| `INTEGER1 -eq INTEGER2` | INTEGER1, INTEGER2' ye sayısal olarak eşit değerlere sahiptir. |
| `INTEGER1 -gt INTEGER2` | INTEGER1, INTEGER2'den daha fazladır.                          |
| `INTEGER1 -lt INTEGER2` | INTEGER1, INTEGER2'den daha azdır.                             |
| `-d FILE`               | FILE belirtilen konumda bulunur..                              |
| `-e FILE`               | FILE vardır.                                                   |
| `-r FILE`               | FILE vardır ve okuma izinleri geçerlidir..                     |
| `-s FILE`               | FILE vardır ve içerisi boş değildir.                           |
| `-w FILE`               | FILE vardır ve yazma izinleri geçerlidir.                      |
| `-x FILE`               | FILE vardır ve *execute* izinleri geçerlidir..                 |
| `&&`                    | Ve operatörü.                                                  |
| `||`                    | Veya operatörü.                                                |

### If-Elif-Else

```shell
if [ "$x" -lt "$y" ] then
    echo Test işlemi başarılı.

elif [$2 == 'yes'] then
    echo İkinci parametre onaylandı.

else
    echo Hiçbir parametre onaylanmadı.

fi
```

### Switch-Case

```shell
#!/bin/bash
mevcut_bosluk=$( df -h | awk '{ print $5 }' | sort -n | tail -n 1 | sed 's/%//' )
case $mevcut_bosluk in
    [1-5]*)
        echo Bir çok alan mevcut.
        ;;
    [6-7]*)
        echo Diskin %60-%70 arasında doluluk oranı bulunuyor.
        ;;
    8*)
        echo Diskin %80 arasında doluluk oranı bulunuyor.
        ;;
    9*)
        echo Diskin %90 arasında doluluk oranı bulunuyor.
        ;;
    *)
        echo Tam algılanamadı, diskiniz ile ilgili bir problem ile karşılaşılmış olabilir.
        ;;
esac
```

## Argümanlar

- `$0`: Programın adını verir.
- `$1`: Programa gönderilen 1. parametreyi temsil eder.
- `$2`: Programa gönderilen 2. parametreyi temsil eder.
- `$n`: Programa gönderilen n. parametreyi temsil eder.
- `$*`: Programa gönderilen tüm parametreleri temsil eder.

## Genel Yapılar

### Satır satır dosya okuma

```shell
while read f do
    echo "Satır; $f"
done < file
```

### Dosyadan belirtileni arama

```shell
grep foo file
```

### Komut çalıştırma

```shell
komut_1 || komut_2 # Komut 1'i çalıştır, eğer çalışmazsa Komut 2'yi çalıştır.
komut_1 && komut_2 # Komut 1'i  ve Komut 2'yi çalıştır.
```

### Değişken tanımlama

`variable = 'ls'`

### Fonksiyon tanımlama

```shell
doubleit(){
    expr $1\* 2
}
```

## Dosya İşlemleri

| Operatör        | Anlamı                                                               |
| --------------- | -------------------------------------------------------------------- |
| `mv /src /trgt` | *src* klasörünü *trgt* klasörüne taşır.                              |
| `ls a*`         | **a** ile başlayan dosyaları ve klasörleri listeler.                 |
| `ls *a`         | **a** ile biten dosyaları ve klasörleri listeler.                    |
| `ls -ltr`       | Oluşturulma tarihi eskiden yeniye doğru dosya ve klasörleri sıralar. |
| `ls -lSr`       | Boyutlarına göre küçükten büyüğe doğru dosya ve klasörleri sıralar.  |
| `ls -a`         | Gizli ve gizli olmayan tüm dosya ve klasörleri sıralar.              |

## Genel Kullanılan Komutlar

| Komut             | Anlamı                                     |
| ----------------- | ------------------------------------------ |
| `file etc/hosts`  | Belirtilen dosyanın tipini gösterir.       |
| `dirname /bin/ls` | Belirtilen dosyanın klasör adını gösterir. |
| `basename bin/ls` | Dosyanın adını verir.                      |
| `ifconfig -a`     | Tüm ağ özelliklerini gösterir.             |
| `netstat -r`      | Ağda bulunan routerleri gösterir.          |
| `netstat -a`      | Ağda bulunan açık olan portları gösterir.  |
| `wc -l`           | Satırdaki bulunan karakterleri sayar.      |
| `pwd`             | Aktif olan klasör konumunu gösterir.       |
| `date +%Y%m%d`    | Yıl, Ay, Gün gösterir.                     |
| `date +%H%M`      | Saat, Dakika gösterir.                     |
