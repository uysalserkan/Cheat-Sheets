# Git Cheat Sheet

[Bu][git-sitesi] bağlantıyı takip ederek Git versiyon kontrol sisteminin resmi sitesine gidebilirsiniz.

</br></br>

## Ayarlar

</br>

Tüm ayarların değerlerine ve nereden geldiklerini gösterir.

`$ git config --list --show-origin`

Git işlemlerinde gösterilecek adı tanımlıyoruz.

`$ git config --global user.name "Serkan"`

Git işlemlerinde bağlanılacak hesabı tanımlıyoruz.

`$ git config --global user.email "uysalserkan08@gmail.com"`

Komut çıktılarının renkli çıkmasını sağlıyoruz.

##### (Auto yerine `normal`, `red`, `blue`, vs. koyabilir veya hexadecimal kod ile renk belirleyebiliriz.)

`$ git config --global color.ui auto`

Git'in ana dosya düzenleme editörünü belirliyoruz.

`$ git config --global core.editor "nano -w"`

`$ git config --global core.editor "vim"`

`$ git config --global core.editor "'C:/Program Files/Notepad++/notepad++.exe' -multiInst -notabbar -nosession -noPlugin"`

Global atamalarını unset ile kaldırabiliriz.

`$ git config --global unset user.name`

Atamalarınızı tek bir yerden düzenleyebilirsiniz.

`$ git config --global --edit`

Default branch adını tanımlayabiliriz.

`$ git config --global init.defaultBranch main`

Commit komutunun genel taslağını değiştirebiliriz.

`$ git config --global commit.template ~/.gitmessage.txt`

Git komutlarını özel kısaltmalar ile kısaltabilirsiniz.

`$ git config --global alias.glog “log --graph--oneline”`

`git glob` yazarak `git log --graph--oneline` komutunu kısaltabiliriz.

Git hesap ayarlarını saklayabiliriz.

`$ git config --global credential.helper store`

`$ git config --global credential.helper 'store --file ~/.my-credentials'`

`$ git config --global credential.helper cache`

</br></br>

## Proje oluşturma ve Klonlama

Dosya konumunuz içerisinde repository bağlantını oluşturur.

`$ git init`

Belirli bir projeyi bağlantıdan klonlama.

`$ git clone https://github.com/uysalserkan/Cheat-Sheets.git`

`$ git clone ssh://root@uysalserkan.com:[port]/repository.git`

`$ git clone ftp://root@uysalserkan.com:[port]/repository.git`

</br></br>

## Dosya inceleme ve karşılaştırma

Log dosyalarını detaylı inceleme.

`$ git log -n 5 --oneline --graph --stat --decorate`

* `-n 5` ile en son oluşturulan commitleri getirir.

* `--oneline` ile commit mesajlarını tek satırda gösterir ve log kodunu kısaltır.

* `--graph` ile görsel olarak commitlerin durumunu gösterir.

* `--stat` ile hangi log kaydında ne olduğunu daha fazla ayrıntı ile gösterir.

* `--decorate` ile branch adını veya tag'ını ekler.

`$ git log -p --author="Serkan UYSAL" --grep="UYSAL"`

* `-p` ile nelerin değiştiğini ayrıntılı gösterir.
  
* `--author` ile belirlenen kişinin commitlerini gösterir.
  
* `--grep` ile belirtelen kelimeleri veya cümleyi log kayıtlarında arar.
  
Repository'de bulunan tag'ları getirir.

`$ git tag`

Repository'e tag ekler.

`$ git tag -a v0.25`

Repository'den tag kaldırır.

`$ git tag -d v0.25`

[git-sitesi]: https://git-scm.com/
