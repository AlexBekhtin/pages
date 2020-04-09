### Русский язык для git в консоли Windows
В phpStorm есть встроенный терминал, в котором изредка приходится вводить команды git.

Если вы пытаетесь смотреть при этом логи git, то все русскоязычные комментарии будут выглядеть URL-кодированными символами в скобках наподобие  <C8><ED><E8><F6><E8><E0><EB><E8><E7><E0><F6><E8><FF> <EF><F0><EE><E5><EA><F2><E0>.

В интернете есть разные способы «русификации» git, но мне помог простейший способ, состоящий в прописывании в системе переменной окружения LANG=ru_RU.utf8.

После перезагрузки Windows git будет правильно отображать unicode как в консоли Windows, так и в терминале phpStorm.  
http://linux.bolden.ru/git-russian-windows-console/

---
### How to have git log show filenames like svn log -v

For full path names of changed files:

`git log --name-only`

For full path names and status of changed files:

`git log --name-status`

For abbreviated pathnames and a diffstat of changed files:

`git log --stat`

There's a lot more options, [check out the docs](https://git-scm.com/docs/git-log).

https://stackoverflow.com/questions/1230084/how-to-have-git-log-show-filenames-like-svn-log-v
