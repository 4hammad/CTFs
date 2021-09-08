## THM ctf-Pickle Rick
#### Mohammed Hammad | 8th September, 2021

> Server IP: **10.10.157.164**

> Did a nikto and nmap scan.
> Used gobuster for dir enumeration.

### Ports Open
> 22, 80
> tried access machine by ssh using *Username: R1ckRul3s*, *no public key*;

>Viewed source code of index.html found *Username: R1ckRul3s*
>Viewed /robots.txt, found text *Wubbalubbadubdub* 
>/login.php found, tried user name and the text found from robots.txt; 
>Command Panel reached.
>ABLE TO ACCESS MACHINE


>cat command is not allowed
>use less cmd.

>sudo doesn't require password 

>/Sup3rS3cretPickl3Ingred.txt contains **mr. meeseek hair** *This is the first flag*

>Searched in /home/rick/"second ingredients" found **1 jerry tear** *This is the second flag*

>root seems an interesting dir
>used sudo ls /* to list out contents of everything, found *3rd.txt* in /root
>*3rd.txt* contains **fleeb juice** which is *the third and final flag*