# Telnet Acesso a Computadores para validar quais serviços ativos(válido):

Protocolo de Rede **TELNET** permite a comunicação em interface de texto.

É possivel verificar se um serviço ou porta está ativo (válido) em determinado computador.

Existe o protocolo **Telnet na porta 23** tanto em Windows e Linux.

O protocolo Telnet não é um protocolo seguro com criptografia de dados.

Exemplo 1:

Instalando o Telnet no Linux.

```
└─$ sudo apt install telnet
[sudo] password for kali:
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following packages were automatically installed and are no longer required:
  libperl5.34 perl-modules-5.34
Use 'sudo apt autoremove' to remove them.
The following additional packages will be installed:
  inetutils-telnet
The following NEW packages will be installed:
  inetutils-telnet telnet
0 upgraded, 2 newly installed, 0 to remove and 21 not upgraded.
Need to get 131 kB of archives.
After this operation, 286 kB of additional disk space will be used.
Do you want to continue? [Y/n] Y
Get:1 http://kali.download/kali kali-rolling/main amd64 inetutils-telnet amd64 2:2.4-1 [105 kB]
Get:2 http://http.kali.org/kali kali-rolling/main amd64 telnet all 0.17+2.4-1 [26.2 kB]
Fetched 131 kB in 1s (91.6 kB/s)
Selecting previously unselected package inetutils-telnet.
(Reading database ... 68265 files and directories currently installed.)
Preparing to unpack .../inetutils-telnet_2%3a2.4-1_amd64.deb ...
Unpacking inetutils-telnet (2:2.4-1) ...
Selecting previously unselected package telnet.
Preparing to unpack .../telnet_0.17+2.4-1_all.deb ...
Unpacking telnet (0.17+2.4-1) ...
Setting up inetutils-telnet (2:2.4-1) ...
update-alternatives: using /usr/bin/inetutils-telnet to provide /usr/bin/telnet (telnet) in auto mode
Setting up telnet (0.17+2.4-1) ...
Processing triggers for man-db (2.11.0-1+b1) ...
Scanning processes...
Scanning processor microcode...
Scanning linux images...
```

Exemplo 2:

Analise de uma maquina com o protocolo telnet verificando se um servidor Web está ativo (válido) dentro da rede:

![image](https://user-images.githubusercontent.com/33209944/210155549-0c2dde81-4262-4494-bc39-0f641be4a286.png)

Conforme a figura acima mostra conseguimos identificar a versão do servidor web **Server: nginx/1.23.2** na **porta 80**.



