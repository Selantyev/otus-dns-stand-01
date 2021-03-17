# otus-dns-stand-01

Настраиваем split-dns
Взят стенд https://github.com/erlong15/vagrant-bind

Добавлен еще один сервер client2
В зону dns.lab добавлены имена:

web1 - смотрит на client
web2 - смотрит на client2

Добавлена ещё одна зона dnsnew.lab, в ней добавлена запись:

www - смотрит на client и client2

Настроен split-dns
client - видит обе зоны (??? но в зоне dns.lab только web1 ???)

client2 - видит только dns.lab
