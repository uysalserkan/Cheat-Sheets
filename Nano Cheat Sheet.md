# Nano Cheat Sheet

:grey_question: GNU Nano **terminal üzerinde çalışan** bir metin düzenleme editörüdür ve **C** dilinde yazılmıştır.

## Bölümler

- [Nano Cheat Sheet](#nano-cheat-sheet)
  - [Bölümler](#bölümler)
    - [Dosya İşlemleri](#dosya-i̇şlemleri)
    - [Düzenleme İşlemleri](#düzenleme-i̇şlemleri)
    - [Araştırma ve Yerleştirme İşlemleri](#araştırma-ve-yerleştirme-i̇şlemleri)
    - [Silme İşlemleri](#silme-i̇şlemleri)
    - [Özel Operasyon İşlemleri](#özel-operasyon-i̇şlemleri)
    - [Dosya İçerisinde Hareket İşlemleri](#dosya-i̇çerisinde-hareket-i̇şlemleri)
    - [Dosya İçerisinde Özel Hareket İşlemleri](#dosya-i̇çerisinde-özel-hareket-i̇şlemleri)
    - [Bilgilendirme İşlemleri](#bilgilendirme-i̇şlemleri)
    - [Diğer İşlemler](#diğer-i̇şlemler)

</br>

### Dosya İşlemleri

|  Komutlar  | Açıklama                                                                         |
| :--------: | -------------------------------------------------------------------------------- |
| `CTRL + S` | Aktif dosyada yaptığınız değişiklikleri kayıt eder.                              |
| `CTRL + O` | Aktif dosyayı aynı isim ile mi yoksa farklı isim ile mi kayıt edeceğinizi sorar. |
| `CTRL + R` | Aktif dosyanın içerisine diğer bir dosyanın tamamını yazdırma işlemi.            |
| `CTRL + X` | Aktif dosyanın kapatılmasını sağlar.                                             |

</br>

### Düzenleme İşlemleri

|  Komutlar  | Açıklama                                                                        |
| :--------: | ------------------------------------------------------------------------------- |
| `CTRL + K` | İşaretçinin bulunduğu satırı kopyalayıp keser.                                  |
| `CTRL + M` | Bir üst satıra bir satır boşluğu ekler.                                         |
| `ALT + 6`  | İşaretçinin bulunduğu satırı kopyalar.                                          |
| `CTRL + U` | İşaretçinin bulunduğu satırın altına kopyalanan metni yapıştırır.               |
| `ALT + T`  | İşaretçinin bulunduğu satırdan en alt satıra kadar kopyalayıp keser.            |
| `ALT + 3`  | İşaretçinin bulunduğu satırı yorum satırı yapar veya yorum satırından çıkartır. |
| `CTRL + ]` | Yazılan komutu tamamlar.                                                        |
| `ALT + U`  | Son işlemi geri alır.                                                           |
| `ALT + E`  | Geri alınan son işlemi tekrar uygular.                                          |

</br>

### Araştırma ve Yerleştirme İşlemleri

|  Komutlar  | Açıklama                                                  |
| :--------: | --------------------------------------------------------- |
| `CTRL + Q` | İşaretçinin arkasında kalan yer için girilen yazıyı arar. |
| `CTRL + W` | İşaretçinin önünde kalan yer için girilen yazıyı arar.    |
| `ALT + Q`  | Aranan yazıyı geriye dönük olarak arar.                   |
| `ALT + W`  | Aranan yazıyı ileriye dönük olarak arar.                  |
| `ALT + R`  | Aranacak olan yazıyı diğer yazıyla değiştirir.            |

</br>

### Silme İşlemleri

|     Komutlar      | Açıklama                                      |
| :---------------: | --------------------------------------------- |
|    `CTRL + H`     | İşaretçi öncesindeki karakteri siler.         |
|    `CTRL + D`     | İşaretçi sonrasındaki karakteri siler.        |
| `ALT + Backspace` | İşaretçinin solundaki kelimeyi siler.         |
|   `CTRL + Del`    | İşaretçinin sağındaki kelimeyi siler.         |
|    `ALT + Del`    | İşaretçinin bulunduğu satırı siler.           |
|     `ALT + T`     | İşaretçinin bulunduğu yerden ilerisini siler. |

</br>

### Özel Operasyon İşlemleri

:warning: Eğer doğru ayarlamaları yaptıysanız bu komutlar çalışacaktır.

|  Komutlar  | Açıklama                                          |
| :--------: | ------------------------------------------------- |
| `CTRL + T` | Komut çalıştır.                                   |
| `CTRL + J` | :question:                                        |
| `ALT + J`  | :question:                                        |
| `ALT + B`  | Yazım kurallarını kontrol eder.                   |
| `ALT + F`  | Tanımladığınız formatter/fixer sistemini uygular. |
| `ALT + :`  | Macro kayıt ve durdurma.                          |
| `ALT + ;`  | Makroyu tekrarlama.                               |

</br>

### Dosya İçerisinde Hareket İşlemleri

|          Komutlar          | Açıklama                               |
| :------------------------: | -------------------------------------- |
|         `CTRL + B`         | İşaretçi bir karakter geri gider.      |
|         `CTRL + F`         | İşaretçi bir karakter ileri gider.     |
|         `CTRL + ←`         | İşaretçi bir kelime geri gider.        |
| `CTRL + →` veya `CTRL + 2` | İşaretçi bir kelime ileri gider.       |
|         `CTRL + A`         | İşaretçi satır başına gider.           |
|         `CTRL + E`         | İşaretçi satır sonuna gider.           |
|         `CTRL + P`         | İşaretçi bir satır yukarıya gider.     |
|         `CTRL + N`         | İşaretçi bir satır aşağıya gider.      |
|         `CTRL + ↑`         | İşaretçi bir blok geri gider.          |
|         `CTRL + ↓`         | İşaretçi bir blok ileri gider.         |
|         `CTRL + Y`         | İşaretçi bir sayfa ileri gider.        |
|         `CTRL + V`         | İşaretçi bir sayfa geri gider.         |
|         `ALT + \`          | Buffer başına gider.                   |
|         `ALT + /`          | Buffer sonuna gider.                   |
|   `ALT + 9 veya ALT + 7`   | Üst satır başlıklarına gider.          |
|         `ALT + 8`          | Alt satır başlıklarına gider.          |
|         `ALT + 0`          | Alta doğru satır boşluklarına ilerler. |

</br>

### Dosya İçerisinde Özel Hareket İşlemleri

|         Komutlar          | Açıklama                               |
| :-----------------------: | -------------------------------------- |
| `Alt + G` veya `CTRL + 7` | İşaretçi belirtilen satıra gider.      |
|         `Alt + ]`         | İşaretçi braketin diğer kısmına gider. |
|         `Alt + ↑`         | Ekran görüntüsünü yukarıya kaydırır.   |
|         `Alt + ↓`         | Ekran görüntüsünü aşağıya kaydırır.    |
|         `Alt + <`         | :question:                             |
|         `Alt + >`         | :question:                             |
|         `Alt + S`         | :question:                             |
|         `Alt + L`         | :question:                             |
|         `Alt + Z`         | :question:                             |

</br>

### Bilgilendirme İşlemleri

|  Komutlar  | Açıklama                                                               |
| :--------: | ---------------------------------------------------------------------- |
| `Ctrl + C` | İşaretçi satır/kelime pozisyonunu gösterir.                            |
| `Alt + D`  | Dosyada bulunan toplam kelime, satır, karakter istatistiğini gösterir. |
| `Ctrl + G` | Yardım sayfasını gösterir.                                             |
| `ALT + Y`  | Syntaxları renklendirmeyi açıp/kapatır.                                |
| `ALT + X`  | Yardımcı modu açıp/kapatır.                                            |
| `ALT + M`  | Mouse destek modu açıp/kapatır.                                        |
| `ALT + C`  | Sabit imleç modunu açıp/kapatır.                                       |

</br>

### Diğer İşlemler

|   Komutlar    | Açıklama                                         |
| :-----------: | ------------------------------------------------ |
|   `Alt + i`   | Otomatik boşluk bırakma işlemini gerçekleştirir. |
|   `Alt + P`   | Boşlukları . olarak gösterir.                    |
|   `Alt + J`   | Alt alta boşluksuz satırları yan yana dizer.     |
|   `Alt + O`   | Tab karakterlerini space karakterine çevirir.    |
|   `Alt + A`   | İşaretleme aracını açıp kapatır.                 |
|     `Tab`     | Bir satır boşluk bırakır.                        |
| `Shift + Tab` | Bir satır boşluğu kaldırır.                      |
|   `Alt + N`   | Satır numaralarını açıp kapatır.                 |
|   `Alt + P`   | Boşlukların gösterimini açıp kapatır.            |
|   `Alt + V`   | Özel tuş girdisi yazdırabilirsiniz.              |
|  `Ctrl + L`   | Ekranı yeniler.                                  |
|  `Ctrl + Z`   | Nanoyu durdurur.                                 |

</br>

:pray: Eğer :question: işaretlerinin yerine uygun ifade olduğunu düşündüğünüz bir açıklama varsa veya eklenecek komutlar varsa isterseniz [request][request-link] açabilir veya [linkedin][linkedin-link] üzerinden benimle iletişime geçebilirsiniz.

[request-link]: https://github.com/uysalserkan/Cheat-Sheets/pulls
[linkedin-link]: https://linkedin.com/in/uysalserkan
