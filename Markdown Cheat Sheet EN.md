# Markdown Cheat Sheet

## Sections

* [Headline](#headline)
* [Text Styles](#text-styles)
* [Listing](#listing)
* [Specified Examples](#specified-topics)
* [Emojies](#emojies)

</br>

## Headline

##### [(examples)](#headline-examples)

</br></br>

|    Kod     |                       Açıklama                       |
| :--------: | :--------------------------------------------------: |
|   *`#`*    | **Main Headline** _32px_ </br> Comes with underline. |
|   *`##`*   |               **Page Headline** _24px_               |
|  *`###`*   |           **Statement Headline** _18.72px_           |
|  *`####`*  |                **Headline 4** _16px_                 |
| *`#####`*  |               **Headline 5** _13.28px_               |
| *`######`* |               **Headline 6** _10.72px_               |

* * *

</br></br>

## Text Styles

##### [(Examples)](#text-style-examples)

</br></br>

|      Kod       |    Açıklama     |
| :------------: | :-------------: |
|   *`*YAZI*`*   |     Italic      |
|   *`_YAZI_`*   |     Italic      |
|  *`__YAZI__`*  |      Bold       |
|  *`**YAZI**`*  |      Bold       |
| *`***YAZI***`* | Bold and Italic |
| *`___YAZI___`* | Bold and Italic |
|  *`~~YAZI~~`*  |  Strikethrough  |
|   *`> YAZI`*   |      Quote      |
|  *`> > YAZI`*  |  Double Quote   |
| ``` `YAZI` ``` |  Oneline code   |
|   *`- - -`*    | Horizontal rule |
|   *`* * *`*    | Horizontal rule |

* * *

</br></br>

## Listing

##### [(examples)](#listing-examples)

</br></br>

|        Kod         |             Açıklama             |
| :----------------: | :------------------------------: |
|  *`1.`</br>`2.`*   |        List with numbers.        |
|       *`*`*        | List with asterisk symbol. (Dot) |
|       *`+`*        |   List with plus symbol. (Dot)   |
|       *`-`*        |   List with dash symbol. (Dot)   |
| *`1.`</br></t>`*`* |     Listing with inner list.     |

* * *

</br></br>

## Specified Topics

##### [(examples)](#specified-examples)

</br></br>

|                                       Kod                                        |                                Açıklama                                |
| :------------------------------------------------------------------------------: | :--------------------------------------------------------------------: |
|                               *`[Yazı](bağlantı)`*                               |                         Adding Link operation.                         |
|                       *`![Alt-Yazı](fotoğraf-bağlantısı)`*                       |                        Adding Image operation.                         |
| *`[Yazı][bağlantı]`</br>`[bağlantı]: https://github.com/uysalserkan "Bağlantı"`* | Another link operation.</br>We define the links at bottom of document. |
|                            *`Adı`</br>`: Açıklaması`*                            |                    We could use when make a define.                    |
|               *`| C1 | C2 |`</br>`| -- | -- |`</br> `| XX | XX |`*               |      Creating table. </br>(C1, C2 are columns name, XXs are row.)      |
|        *`~~~Python`</br>`{`</br>`//Çok Satırlı Kodlar`</br>`}`</br>`~~~`*        |    Fenced Code Block. (Multiline codes and we can define language)     |
|      *` ```Python`</br>`{`</br>`//Çok Satırlı Kodlar`</br>`}`</br>` ``` `*       |    Fenced Code Block. (Multiline codes and we can define language)     |
|                               *`- [ ] Yapılmamış`*                               |                             Unchecked box.                             |
|                               *`- [ X ] Yapılmış`*                               |                              Checked box.                              |

* * *

</br></br>

## Emojies

</br>

|                     Kod                      |          İfade          |
| :------------------------------------------: | :---------------------: |
|          `:slightly_smiling_face:`           | :slightly_smiling_face: |
|             `:money_mouth_face:`             |   :money_mouth_face:    |
|                 `:thinking:`                 |       :thinking:        |
|                   `:hand:`                   |         :hand:          |
|                    `:+1:`                    |          :+1:           |
|                `:handshake:`                 |       :handshake:       |
|               `:writing_hand:`               |     :writing_hand:      |
|                 `:moneybag:`                 |       :moneybag:        |
| *[Click][emojibağlantısı]* for more emojies. |         :link:          |

</br></br>

## Examples

</br>

### Headline Examples

</br>

#  Main headline

##  Page headline

###  Statement headline

####  Headline 4

#####  Headline 5

###### Headline 6

</br></br>

### Text Style Examples

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

### Listing Examples

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

### Specified Examples

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
[emojibağlantısı]: https://www.webfx.com/tools/emoji-cheat-sheet/