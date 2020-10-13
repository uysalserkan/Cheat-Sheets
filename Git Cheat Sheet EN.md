# Git Cheat Sheet

You could explore and install git version control system followed by [this][git-sitesi] link.

</br></br>

## Settings

</br>

You can show settings and paths.

`$ git config --list --show-origin`

Shows name when you commit.

`$ git config --global user.name "Serkan"`

Adding default e-mail address to account.

`$ git config --global user.email "uysalserkan08@gmail.com"`

Printing colourful commands
##### (You can set `normal`, `red`, `blue`, etc. or hexadecimal code instead of auto.)

`$ git config --global color.ui auto`

You can decide text editor on terminal.

`$ git config --global core.editor "nano -w"`

`$ git config --global core.editor "vim"`

`$ git config --global core.editor "'C:/Program Files/Notepad++/notepad++.exe' -multiInst -notabbar -nosession -noPlugin"`

You can unset global sets.

`$ git config --global unset user.name`

You can set your sets on one code.

`$ git config --global --edit`

You could configure default branch name.

`$ git config --global init.defaultBranch main`

Change default commit template.

`$ git config --global commit.template ~/.gitmessage.txt`

You can add alias.

`$ git config --global alias.glog “log --graph--oneline”`

`git glob` alias `git log --graph--oneline` this command.

You can store your account configurations.

`$ git config --global credential.helper store`

`$ git config --global credential.helper 'store --file ~/.my-credentials'`

`$ git config --global credential.helper cache`

</br></br>

## Creating or cloning projects

You can initialize git configurations.

`$ git init`

Clone a project with URL.

`$ git clone https://github.com/uysalserkan/Cheat-Sheets.git`

`$ git clone ssh://root@uysalserkan.com:[port]/repository.git`

`$ git clone ftp://root@uysalserkan.com:[port]/repository.git`

</br></br>

## Comparing and investigating files

Log files with long detailes.

`$ git log -n 5 --oneline --graph --stat --decorate`

  * `-n 5` last 5 commits.

  * `--oneline` short commit messages.

  * `--graph` graphical commits.
  
  * `--stat` long description commits.
  
  * `--decorate` show branch names and tags.

`$ git log -p --author="Serkan UYSAL" --grep="UYSAL" `

  * `-p` showing differences.
  
  * `--author` showing this author commits.
  
  * `--grep` searching word(s) in log files.
  
Getting tags.

`$ git tag`

Adding tag on repository.

`$ git tag -a v0.25`

Removing tag on repository.

`$ git tag -d v0.25`

[git-sitesi]: https://git-scm.com/