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

<!-- ___test___

***test2***

Here's a sentence with a footnote. [^1]

### My Great Heading {#başlıklar}

* Bullet lists are easy too

- Another one

+ Another one

+ [ ] Y

* * *

Cplusplus:

    //Code
    which(is_easy) to_remember();
And now some code:

    // Code is just text indented a bit
    which(is_easy) to_remember();

~~~CPP
// Markdown extra adds un-indented code blocks too

if (this_is_more_code == true && !indented) {
  // tild wrapped code blocks, also not indented
}
~~~

- - -

```CPP
// Markdown extra adds un-indented code blocks too

if (this_is_more_code == true && !indented) {
    // tild wrapped code blocks, also not indented
}
```

[^1]: This is the footnote.

* [x] Write the press release
* [ ] Update the website
* [ ] Contact the media
* [ ] Test

```plain-text
TEST TEST TEST
```

> Alıntıla
> > Çift Alıntıla
> > Çift 2
>
> xdxdd
> test
> xdxd

> Email-style angle brackets are used for blockquotes.
>> You can also nest them.
>>
> * You can quote a list.
> * Etc.

> To break the nested blockquote, add a space between lines.


xx
:  Test

– [x] Task to do

term
: definition

~~Flat is world~~

– [ x ] done

Here's a sentence with a footnote. [^1]

Text serkan.

[^1]: This is the footnote.
```json
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

---

x

***

x

___





#### Header 4

##### Header 5

###### Header 6


*[HTML]: HyperText Markup Language





 -->

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

</br></br>

### Listeleme Örnekleri

</br></br>

### Gelismis Ornekler

Burada herhangi [bir link][1] ve diğer [link][2] bulunuyor.

[1]: http://github.com/uysalserkan "Title"
[2]: http://github.com/uysalserkan "Title"

Veya satır içi [link](http://github.com/uysalserkan) de bulunabilir.

