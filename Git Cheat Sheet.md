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

Atamalarınızı tek bir yerden düzenleyebilirsiniz.

`$ git config --global --edit`

Default branch adını tanımlayabiliriz.

`$ git config --global init.defaultBranch main`

Commit komutunun genel taslağını değiştirebiliriz.

`$ git config --global commit.template ~/.gitmessage.txt`

Git komutlarını özel kısaltmalar ile kısaltabilirsiniz.

`git config --global alias.glog “log --graph--oneline”`

`git glob` yazarak `git log --graph--oneline` komutunu kısaltabiliriz.

[git-sitesi]: https://git-scm.com/