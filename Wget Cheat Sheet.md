# Markdown Cheat Sheet

## Bölümler

## :warning: Basit Operasyonlar

URL'den dosyayı indir

~~~bash
wget URL-bağlantısı
~~~

URL'den dosyayı belirlediğiniz isim ile indirir

~~~bash
wget -o isim.zip URL-bağlantısı
~~~

Birden fazla dosya indir

~~~bash
wget URL-bağlantısı-1 URL-bağlantısı-2
~~~

Dosyada bulunan linklerdeki dosyaları indir

~~~bash
wget -i indirilecek/linkler.txt
~~~

Durdurulan indirmeyi devam et

~~~bash
wget -c URL-durduruldu
~~~

URL'deki dosyayı arka planda indir

~~~bash
wget -b URL-bağlantısı
~~~

URL'deki dosyayı arka planda indir ve logları dosyaya yaz

~~~bash
wget -b /wget/logs.txt URL-bağlantısı
~~~

Dosya indirme hızını sınırla

~~~bash
wget --limit-rate=250k URL-bağlantısı
~~~

URL'deki dosyayı belirtilen defa deneme

~~~bash
wget --tries=75 URL-bağlantısı
~~~

URL'deki bağlantı belirtilen boyutu geçerse durdur

~~~bash
wget -Q10m -i download-list.txt
~~~

</br>

## :bookmark: Tüm Operasyonlar

**will be here**
