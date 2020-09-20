# Markdown Cheat Sheet

## Bölümler

* [Başlıklar](#başlıklar)
* [Yazı Stilleri](#yazı-sitilleri)
* [Listeleme](#listeleme)
* [Gelismis Komutlar](#gelişmiş-komutlar)

</br>

## Başlıklar

##### [(örnekler)](#başlık-örnekleri)

</br></br>

|    Kod     |                       Açıklama                       |
| :--------: | :--------------------------------------------------: |
|   *`#`*    | **Ana Başlık** _32px_ </br> Altında çizgi ile gelir. |
|   *`##`*   |               **Sayfa Başlığı** _24px_               |
|  *`###`*   |             **Satır Bağlığı** _18.72px_              |
|  *`####`*  |               **Alt Başlık 1** _16px_                |
| *`#####`*  |              **Alt Başlık 2** _13.28px_              |
| *`######`* |              **Alt Başlık 3** _10.72px_              |

* * *

</br></br>

## Yazı Sitilleri

##### [(örnekler)](#yazı-stilleri-örnekleri)

</br></br>

|      Kod       |             Açıklama              |
| :------------: | :-------------------------------: |
|   *`*YAZI*`*   |             Eğik yazı             |
|   *`_YAZI_`*   |             Eğik yazı             |
|  *`__YAZI__`*  |            Kalın yazı             |
|  *`**YAZI**`*  |            Kalın yazı             |
| *`***YAZI***`* |       Kalın ve italik yazı        |
| *`___YAZI___`* |       Kalın ve italik yazı        |
|  *`~~YAZI~~`*  |          Üstü çizik yazı          |
|   *`> YAZI`*   |          Yazıyı Alıntıla          |
|  *`> > YAZI`*  | Yazıyı Alıntı İçerisinde Alıntıla |
| ``` `YAZI` ``` |    Tek Satırlık Kod Satırları     |
|   *`- - -`*    |           Satır çizgisi           |
|   *`* * *`*    |           Satır çizgisi           |

* * *

</br></br>

## Listeleme

##### [(örnekler)](#listeleme-örnekleri)

</br></br>

|        Kod         |                                              Açıklama                                              |
| :----------------: | :------------------------------------------------------------------------------------------------: |
|  *`1.`</br>`2.`*   |                                 Numaraları seri olarak listeleme.                                  |
|       *`*`*        |                             Asterisk işareti ile lisleleme. (Noktasal)                             |
|       *`+`*        |                               Artı işareti ile lisleleme. (Noktasal)                               |
|       *`-`*        |                               Eksi işareti ile lisleleme. (Noktasal)                               |
| *`1.`</br></t>`*`* | Bir operatörün ardıntan tab boşluğu bıraktıktan sonra </br>diğer operatör ile alt liste oluşturma. |

* * *

</br></br>

## Gelişmiş Komutlar

##### [(örnekler)](#gelismis-ornekler)

</br></br>

|                                       Kod                                        |                                               Açıklama                                                |
| :------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------: |
|                               *`[Yazı](bağlantı)`*                               |                                   Yazı üzerine link bağlama işlemi.                                   |
|                       *`![Alt-Yazı](fotoğraf-bağlantısı)`*                       |                                        Fotoğraf ekleme işlemi.                                        |
| *`[Yazı][bağlantı]`</br>`[bağlantı]: https://github.com/uysalserkan "Bağlantı"`* |            Yazı üzerine link bağlama işlemi.</br>Bağlantıyı dosyaların altında tanımlarız.            |
|                            *`Adı`</br>`: Açıklaması`*                            |                           Bir şeyin tanımını göstermek için kullanılabilir.                           |
|               *`| C1 | C2 |`</br>`| -- | -- |`</br> `| XX | XX |`*               |        Tablo oluşturma. </br>(C1, C2 Kolon adlarını, XX satırları ise sütünları temsil ediyor)        |
|        *`~~~Python`</br>`{`</br>`//Çok Satırlı Kodlar`</br>`}`</br>`~~~`*        | Çok satırlı kodlarınızı böyle gösterebilirsiniz. </br> Python yerine istediğiniz dili yazabilirsiniz. |
|      *` ```Python`</br>`{`</br>`//Çok Satırlı Kodlar`</br>`}`</br>` ``` `*       | Çok satırlı kodlarınızı böyle gösterebilirsiniz. </br> Python yerine istediğiniz dili yazabilirsiniz. |
|                               *`- [ ] Yapılmamış`*                               |                                 İşaretsiz checkbox oluşturma işlemi.                                  |
|                               *`- [ X ] Yapılmış`*                               |                                  İşaretli checkbox oluşturma işlemi.                                  |

</br>

## Örnekler

</br>

### Başlık Örnekleri

</br>

# `#` Ana Başlık

## `##` Sayfa Başlığı

### `###` Satır Başlığı

#### `####` Başlık 1

##### `#####` Başlık 2

###### `######` Başlık 3

</br></br>

### Yazı Stilleri Örnekleri

</br>

*Eğik Yazı 1*

_Eğik Yazı 2_

**Kalın Yazı 1**

__Kalın Yazı 2__

***Kalın ve Eğik Yazı 1***

___Kalın ve Eğik Yazı 2___

~~Üzeri Çizili Yazı~~

</br>

> `>` Bu işaret ile
> alıntı yapabilirsiniz.
> > `> >` böyle ise iç alıntıya
> geçebilirsiniz.
> >
> ve bir satır `> >` bu şekilde boşluk bırakarak alt alıntıya devam edebilrsiniz.

> Bir satır boşluk bırakarak diğer bir
> alıntıya geçiş yapabilirsiniz.

</br>

` `` işareti ile tek satırlık kod yazabilrsiniz. `

</br>

veya kodlarınızı böyle:

    yazabilirsiniz. Fakat bu durumda 
    her hangi bir dil belirtemiyorsunuz.

</br>

`- - - işareti ile çizgi`

- - -

`* * * işareti ile çizgi`

* * *

</br></br>

### Listeleme Örnekleri

</br>

1. Sayısal
2. Olarak
3. Artan

</br>

* Noktasal
- Olarak
+ Artan

</br>

* İç
  1. İçe
     * Geçmiş
       1. Listeleri
          * Kombinleyebilirsiniz.

</br></br>

### Gelismis Ornekler

</br>

Burada herhangi [bir link][1] ve diğer [link][2] bulunuyor.

</br>

[1]: http://github.com/uysalserkan "Title"
[2]: http://github.com/uysalserkan "Title"

</br>

Veya satır içi [link](http://github.com/uysalserkan) de bulunabilir.

</br>

![GitHub Profil Fotoğrafı](https://avatars2.githubusercontent.com/u/24881389?s=460&u=0a6812427c32c13988824dbb597508482f71b66f&v=4)

</br>

Serkan
:  Yapay zeka ve makine öğrenmesi ile ilgileniyorum.

</br>

**Mail Adresi**
: uysalserkan08@gmail.com

</br>

# Ana Başlık

## Sayfa Başlığı

### Satır Başlığı

#### Başlık 1

##### Başlık 2

###### Başlık 3

</br>

| *Birinci Kolon* | İkinci Kolon | Üçüncü Kolon |
| :-------------: | -----------: | :----------- |
|     Girdi 1     |  ~~Girdi 2~~ | Girdi 1.2    |
|     Girdi 3     |      Girdi 4 | Girdi 3.4    |
|     Girdi 4     |      Girdi 6 | Girdi 4.6    |

</br>

```Python
def main():
    for index in range(25):
        print("Serkan: {}".format(index))

if __name__ == "__main__":
    print("Main fonksiyon başlatılıyor..")
    # Buraya yorum satırları koyabilirsiniz..
    main()
```

</br>

~~~CPP
int main(){
  for(int i=0;i<25;i++){
    cout << "Serkan: "<< i << endl;
  }
}
~~~

</br>

* [ ] Bu görev __yapılacak..__
* [x] Bu görev yapıldı..
* [x] [Dış link verebilirsiniz.][myLinkedin]
* [ ] ~~Bu görevden vazgeçildi..~~

[myLinkedin]: https://linkedin.com/in/uysalserkan
