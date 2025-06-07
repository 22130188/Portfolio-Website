# Portfolio Website
( https://www.youtube.com/watch?v=gWVIIU1ev0Y&t=5s ) .  

   ,     #_
   ~\_  ####_        Amazon Linux 2023
  ~~  \_#####\
  ~~     \###|
  ~~       \#/ ___   https://aws.amazon.com/linux/amazon-linux-2023
   ~~       V~' '->
    ~~~         /
      ~~._.   _/
         _/ _/
       _/m/'
[ec2-user@ip-172-31-0-187 ~]$ sudo su -
[root@ip-172-31-0-187 ~]# yum update -y
Amazon Linux 2023 Kernel Livepatch repository                                                                                          123 kB/s |  16 kB     00:00    
Dependencies resolved.
Nothing to do.
Complete!
[root@ip-172-31-0-187 ~]# yum install -y httpd
Last metadata expiration check: 0:00:46 ago on Sat Jun  7 19:22:14 2025.
Dependencies resolved.
=======================================================================================================================================================================
 Package                                     Architecture                   Version                                          Repository                           Size
=======================================================================================================================================================================
Installing:
 httpd                                       x86_64                         2.4.62-1.amzn2023                                amazonlinux                          48 k
Installing dependencies:
 apr                                         x86_64                         1.7.5-1.amzn2023.0.4                             amazonlinux                         129 k
 apr-util                                    x86_64                         1.6.3-1.amzn2023.0.1                             amazonlinux                          98 k
 generic-logos-httpd                         noarch                         18.0.0-12.amzn2023.0.3                           amazonlinux                          19 k
 httpd-core                                  x86_64                         2.4.62-1.amzn2023                                amazonlinux                         1.4 M
 httpd-filesystem                            noarch                         2.4.62-1.amzn2023                                amazonlinux                          14 k
 httpd-tools                                 x86_64                         2.4.62-1.amzn2023                                amazonlinux                          81 k
 libbrotli                                   x86_64                         1.0.9-4.amzn2023.0.2                             amazonlinux                         315 k
 mailcap                                     noarch                         2.1.49-3.amzn2023.0.3                            amazonlinux                          33 k
Installing weak dependencies:
 apr-util-openssl                            x86_64                         1.6.3-1.amzn2023.0.1                             amazonlinux                          17 k
 mod_http2                                   x86_64                         2.0.27-1.amzn2023.0.3                            amazonlinux                         166 k
 mod_lua                                     x86_64                         2.4.62-1.amzn2023                                amazonlinux                          61 k

Transaction Summary
=======================================================================================================================================================================
Install  12 Packages

Total download size: 2.3 M
Installed size: 6.9 M
Downloading Packages:
(1/12): apr-util-openssl-1.6.3-1.amzn2023.0.1.x86_64.rpm                                                                               476 kB/s |  17 kB     00:00    
(2/12): apr-util-1.6.3-1.amzn2023.0.1.x86_64.rpm                                                                                       2.2 MB/s |  98 kB     00:00    
(3/12): apr-1.7.5-1.amzn2023.0.4.x86_64.rpm                                                                                            2.0 MB/s | 129 kB     00:00    
(4/12): generic-logos-httpd-18.0.0-12.amzn2023.0.3.noarch.rpm                                                                          622 kB/s |  19 kB     00:00    
(5/12): httpd-2.4.62-1.amzn2023.x86_64.rpm                                                                                             1.8 MB/s |  48 kB     00:00    
(6/12): httpd-filesystem-2.4.62-1.amzn2023.noarch.rpm                                                                                  615 kB/s |  14 kB     00:00    
(7/12): httpd-tools-2.4.62-1.amzn2023.x86_64.rpm                                                                                       1.5 MB/s |  81 kB     00:00    
(8/12): httpd-core-2.4.62-1.amzn2023.x86_64.rpm                                                                                         19 MB/s | 1.4 MB     00:00    
(9/12): libbrotli-1.0.9-4.amzn2023.0.2.x86_64.rpm                                                                                      5.5 MB/s | 315 kB     00:00    
(10/12): mailcap-2.1.49-3.amzn2023.0.3.noarch.rpm                                                                                      1.4 MB/s |  33 kB     00:00    
(11/12): mod_lua-2.4.62-1.amzn2023.x86_64.rpm                                                                                          2.3 MB/s |  61 kB     00:00    
(12/12): mod_http2-2.0.27-1.amzn2023.0.3.x86_64.rpm                                                                                    3.1 MB/s | 166 kB     00:00    
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
Total                                                                                                                                   11 MB/s | 2.3 MB     00:00     
Running transaction check
Transaction check succeeded.
Running transaction test
Transaction test succeeded.
Running transaction
  Preparing        :                                                                                                                                               1/1 
  Installing       : apr-1.7.5-1.amzn2023.0.4.x86_64                                                                                                              1/12 
  Installing       : apr-util-openssl-1.6.3-1.amzn2023.0.1.x86_64                                                                                                 2/12 
  Installing       : apr-util-1.6.3-1.amzn2023.0.1.x86_64                                                                                                         3/12 
  Installing       : mailcap-2.1.49-3.amzn2023.0.3.noarch                                                                                                         4/12 
  Installing       : httpd-tools-2.4.62-1.amzn2023.x86_64                                                                                                         5/12 
  Installing       : libbrotli-1.0.9-4.amzn2023.0.2.x86_64                                                                                                        6/12 
  Running scriptlet: httpd-filesystem-2.4.62-1.amzn2023.noarch                                                                                                    7/12 
  Installing       : httpd-filesystem-2.4.62-1.amzn2023.noarch                                                                                                    7/12 
  Installing       : httpd-core-2.4.62-1.amzn2023.x86_64                                                                                                          8/12 
  Installing       : mod_http2-2.0.27-1.amzn2023.0.3.x86_64                                                                                                       9/12 
  Installing       : mod_lua-2.4.62-1.amzn2023.x86_64                                                                                                            10/12 
  Installing       : generic-logos-httpd-18.0.0-12.amzn2023.0.3.noarch                                                                                           11/12 
  Installing       : httpd-2.4.62-1.amzn2023.x86_64                                                                                                              12/12 
  Running scriptlet: httpd-2.4.62-1.amzn2023.x86_64                                                                                                              12/12 
  Verifying        : apr-1.7.5-1.amzn2023.0.4.x86_64                                                                                                              1/12 
  Verifying        : apr-util-1.6.3-1.amzn2023.0.1.x86_64                                                                                                         2/12 
  Verifying        : apr-util-openssl-1.6.3-1.amzn2023.0.1.x86_64                                                                                                 3/12 
  Verifying        : generic-logos-httpd-18.0.0-12.amzn2023.0.3.noarch                                                                                            4/12 
  Verifying        : httpd-2.4.62-1.amzn2023.x86_64                                                                                                               5/12 
  Verifying        : httpd-core-2.4.62-1.amzn2023.x86_64                                                                                                          6/12 
  Verifying        : httpd-filesystem-2.4.62-1.amzn2023.noarch                                                                                                    7/12 
  Verifying        : httpd-tools-2.4.62-1.amzn2023.x86_64                                                                                                         8/12 
  Verifying        : libbrotli-1.0.9-4.amzn2023.0.2.x86_64                                                                                                        9/12 
  Verifying        : mailcap-2.1.49-3.amzn2023.0.3.noarch                                                                                                        10/12 
  Verifying        : mod_http2-2.0.27-1.amzn2023.0.3.x86_64                                                                                                      11/12 
  Verifying        : mod_lua-2.4.62-1.amzn2023.x86_64                                                                                                            12/12 

Installed:
  apr-1.7.5-1.amzn2023.0.4.x86_64                             apr-util-1.6.3-1.amzn2023.0.1.x86_64             apr-util-openssl-1.6.3-1.amzn2023.0.1.x86_64          
  generic-logos-httpd-18.0.0-12.amzn2023.0.3.noarch           httpd-2.4.62-1.amzn2023.x86_64                   httpd-core-2.4.62-1.amzn2023.x86_64                   
  httpd-filesystem-2.4.62-1.amzn2023.noarch                   httpd-tools-2.4.62-1.amzn2023.x86_64             libbrotli-1.0.9-4.amzn2023.0.2.x86_64                 
  mailcap-2.1.49-3.amzn2023.0.3.noarch                        mod_http2-2.0.27-1.amzn2023.0.3.x86_64           mod_lua-2.4.62-1.amzn2023.x86_64                      

Complete!
[root@ip-172-31-0-187 ~]# systemctl status httpd
○ httpd.service - The Apache HTTP Server
     Loaded: loaded (/usr/lib/systemd/system/httpd.service; disabled; preset: disabled)
     Active: inactive (dead)
       Docs: man:httpd.service(8)
[root@ip-172-31-0-187 ~]# mkdir aws_assg3
[root@ip-172-31-0-187 ~]# cd aws_assg3
[root@ip-172-31-0-187 aws_assg3]# wget https://github.com/22130188/Portfolio-Website.git
--2025-06-07 19:25:42--  https://github.com/22130188/Portfolio-Website.git
Resolving github.com (github.com)... 20.27.177.113
Connecting to github.com (github.com)|20.27.177.113|:443... connected.
HTTP request sent, awaiting response... 301 Moved Permanently
Location: https://github.com/22130188/Portfolio-Website [following]
--2025-06-07 19:25:42--  https://github.com/22130188/Portfolio-Website
Reusing existing connection to github.com:443.
HTTP request sent, awaiting response... 200 OK
Length: unspecified [text/html]
Saving to: ‘Portfolio-Website.git’

Portfolio-Website.git                         [ <=>                                                                                 ] 223.23K  --.-KB/s    in 0.02s   

2025-06-07 19:25:43 (10.8 MB/s) - ‘Portfolio-Website.git’ saved [228586]

[root@ip-172-31-0-187 aws_assg3]# ls -lrt
total 224
-rw-r--r--. 1 root root 228586 Jun  7 19:25 Portfolio-Website.git
[root@ip-172-31-0-187 aws_assg3]# wget https://github.com/22130188/Portfolio-Website/archive/refs/heads/main.zip
--2025-06-07 19:31:20--  https://github.com/22130188/Portfolio-Website/archive/refs/heads/main.zip
Resolving github.com (github.com)... 20.27.177.113
Connecting to github.com (github.com)|20.27.177.113|:443... connected.
HTTP request sent, awaiting response... 302 Found
Location: https://codeload.github.com/22130188/Portfolio-Website/zip/refs/heads/main [following]
--2025-06-07 19:31:21--  https://codeload.github.com/22130188/Portfolio-Website/zip/refs/heads/main
Resolving codeload.github.com (codeload.github.com)... 20.27.177.114
Connecting to codeload.github.com (codeload.github.com)|20.27.177.114|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: unspecified [application/zip]
Saving to: ‘main.zip’

main.zip                                      [ <=>                                                                                 ] 604.70K  --.-KB/s    in 0.09s   

2025-06-07 19:31:21 (6.86 MB/s) - ‘main.zip’ saved [619211]

[root@ip-172-31-0-187 aws_assg3]# ls -lrt
total 832
-rw-r--r--. 1 root root 228586 Jun  7 19:25 Portfolio-Website.git
-rw-r--r--. 1 root root 619211 Jun  7 19:31 main.zip
[root@ip-172-31-0-187 aws_assg3]# unzip main.zip
Archive:  main.zip
b5aeab4b1df91e3d2acd74ede36f6359402d8b37
   creating: Portfolio-Website-main/
 extracting: Portfolio-Website-main/README.md  
   creating: Portfolio-Website-main/css/
   creating: Portfolio-Website-main/css/colors/
  inflating: Portfolio-Website-main/css/colors/blue.css  
  inflating: Portfolio-Website-main/css/colors/blue.css.map  
  inflating: Portfolio-Website-main/css/colors/green.css  
  inflating: Portfolio-Website-main/css/colors/green.css.map  
  inflating: Portfolio-Website-main/css/colors/red.css  
  inflating: Portfolio-Website-main/css/colors/red.css.map  
  inflating: Portfolio-Website-main/css/colors/yellow.css  
  inflating: Portfolio-Website-main/css/colors/yellow.css.map  
  inflating: Portfolio-Website-main/css/dark.css  
  inflating: Portfolio-Website-main/css/dark.css.map  
  inflating: Portfolio-Website-main/css/style.css  
  inflating: Portfolio-Website-main/css/style.css.map  
  inflating: Portfolio-Website-main/index.html  
   creating: Portfolio-Website-main/js/
  inflating: Portfolio-Website-main/js/script.js  
   creating: Portfolio-Website-main/plugins/
  inflating: Portfolio-Website-main/plugins/animate.css  
   creating: Portfolio-Website-main/plugins/bootstrap/
  inflating: Portfolio-Website-main/plugins/bootstrap/bootstrap.min.css  
  inflating: Portfolio-Website-main/plugins/bootstrap/bootstrap.min.js  
   creating: Portfolio-Website-main/plugins/isotope/
  inflating: Portfolio-Website-main/plugins/isotope/isotope.pkgd.min.js  
  inflating: Portfolio-Website-main/plugins/jquery-2.2.4.min.js  
  inflating: Portfolio-Website-main/plugins/jquery.nicescroll.min.js  
   creating: Portfolio-Website-main/plugins/slick/
  inflating: Portfolio-Website-main/plugins/slick/README.markdown  
  inflating: Portfolio-Website-main/plugins/slick/ajax-loader.gif  
   creating: Portfolio-Website-main/plugins/slick/fonts/
  inflating: Portfolio-Website-main/plugins/slick/fonts/slick.eot  
  inflating: Portfolio-Website-main/plugins/slick/fonts/slick.svg  
  inflating: Portfolio-Website-main/plugins/slick/fonts/slick.ttf  
  inflating: Portfolio-Website-main/plugins/slick/fonts/slick.woff  
  inflating: Portfolio-Website-main/plugins/slick/slick-theme.css  
  inflating: Portfolio-Website-main/plugins/slick/slick.css  
  inflating: Portfolio-Website-main/plugins/slick/slick.min.js  
   creating: Portfolio-Website-main/plugins/themefisher-fonts/
   creating: Portfolio-Website-main/plugins/themefisher-fonts/css/
  inflating: Portfolio-Website-main/plugins/themefisher-fonts/css/themefisher-fonts.min.css  
   creating: Portfolio-Website-main/plugins/themefisher-fonts/fonts/
  inflating: Portfolio-Website-main/plugins/themefisher-fonts/fonts/themefisher-font.eot  
  inflating: Portfolio-Website-main/plugins/themefisher-fonts/fonts/themefisher-font.svg  
  inflating: Portfolio-Website-main/plugins/themefisher-fonts/fonts/themefisher-font.ttf  
  inflating: Portfolio-Website-main/plugins/themefisher-fonts/fonts/themefisher-font.woff  
[root@ip-172-31-0-187 aws_assg3]# ls -lrt
total 832
drwxr-xr-x. 5 root root     77 Jun  7 19:17 Portfolio-Website-main
-rw-r--r--. 1 root root 228586 Jun  7 19:25 Portfolio-Website.git
-rw-r--r--. 1 root root 619211 Jun  7 19:31 main.zip
[root@ip-172-31-0-187 aws_assg3]# cd Portfolio-Website-main
[root@ip-172-31-0-187 Portfolio-Website-main]# ls -lrt
total 16
drwxr-xr-x. 6 root root   154 Jun  7 19:17 plugins
drwxr-xr-x. 2 root root    23 Jun  7 19:17 js
-rw-r--r--. 1 root root 10607 Jun  7 19:17 index.html
drwxr-xr-x. 3 root root    94 Jun  7 19:17 css
-rw-r--r--. 1 root root     1 Jun  7 19:17 README.md
[root@ip-172-31-0-187 Portfolio-Website-main]# mv * /var/www/html/
[root@ip-172-31-0-187 Portfolio-Website-main]# cd /var/www/html
[root@ip-172-31-0-187 html]# ls -lrt
total 16
drwxr-xr-x. 6 root root   154 Jun  7 19:17 plugins
drwxr-xr-x. 2 root root    23 Jun  7 19:17 js
-rw-r--r--. 1 root root 10607 Jun  7 19:17 index.html
drwxr-xr-x. 3 root root    94 Jun  7 19:17 css
-rw-r--r--. 1 root root     1 Jun  7 19:17 README.md
[root@ip-172-31-0-187 html]# systemctl status httpd
○ httpd.service - The Apache HTTP Server
     Loaded: loaded (/usr/lib/systemd/system/httpd.service; disabled; preset: disabled)
     Active: inactive (dead)
       Docs: man:httpd.service(8)
[root@ip-172-31-0-187 html]# systemctl enable httpd
Created symlink /etc/systemd/system/multi-user.target.wants/httpd.service → /usr/lib/systemd/system/httpd.service.
[root@ip-172-31-0-187 html]# systemctl start httpd


[root@ip-172-31-0-187 html]# yum install -y git
cd ~/aws_assg3
git clone https://github.com/22130188/Portfolio-Website.git
Last metadata expiration check: 0:44:14 ago on Sat Jun  7 19:22:14 2025.
Dependencies resolved.
=======================================================================================================================================================================
 Package                                  Architecture                   Version                                             Repository                           Size
=======================================================================================================================================================================
Installing:
 git                                      x86_64                         2.47.1-1.amzn2023.0.2                               amazonlinux                          54 k
Installing dependencies:
 git-core                                 x86_64                         2.47.1-1.amzn2023.0.2                               amazonlinux                         4.7 M
 git-core-doc                             noarch                         2.47.1-1.amzn2023.0.2                               amazonlinux                         2.8 M
 perl-Error                               noarch                         1:0.17029-5.amzn2023.0.2                            amazonlinux                          41 k
 perl-File-Find                           noarch                         1.37-477.amzn2023.0.6                               amazonlinux                          26 k
 perl-Git                                 noarch                         2.47.1-1.amzn2023.0.2                               amazonlinux                          42 k
 perl-TermReadKey                         x86_64                         2.38-9.amzn2023.0.2                                 amazonlinux                          36 k
 perl-lib                                 x86_64                         0.65-477.amzn2023.0.6                               amazonlinux                          15 k

Transaction Summary
=======================================================================================================================================================================
Install  8 Packages

Total download size: 7.7 M
Installed size: 37 M
Downloading Packages:
(1/8): git-2.47.1-1.amzn2023.0.2.x86_64.rpm                                                                                            1.0 MB/s |  54 kB     00:00    
(2/8): perl-Error-0.17029-5.amzn2023.0.2.noarch.rpm                                                                                    1.7 MB/s |  41 kB     00:00    
(3/8): perl-File-Find-1.37-477.amzn2023.0.6.noarch.rpm                                                                                 1.1 MB/s |  26 kB     00:00    
(4/8): perl-Git-2.47.1-1.amzn2023.0.2.noarch.rpm                                                                                       1.4 MB/s |  42 kB     00:00    
(5/8): perl-TermReadKey-2.38-9.amzn2023.0.2.x86_64.rpm                                                                                 1.1 MB/s |  36 kB     00:00    
(6/8): git-core-2.47.1-1.amzn2023.0.2.x86_64.rpm                                                                                        24 MB/s | 4.7 MB     00:00    
(7/8): perl-lib-0.65-477.amzn2023.0.6.x86_64.rpm                                                                                       361 kB/s |  15 kB     00:00    
(8/8): git-core-doc-2.47.1-1.amzn2023.0.2.noarch.rpm                                                                                    12 MB/s | 2.8 MB     00:00    
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
Total                                                                                                                                   28 MB/s | 7.7 MB     00:00     
Running transaction check
Transaction check succeeded.
Running transaction test
Transaction test succeeded.
Running transaction
  Preparing        :                                                                                                                                               1/1 
  Installing       : git-core-2.47.1-1.amzn2023.0.2.x86_64                                                                                                         1/8 
  Installing       : git-core-doc-2.47.1-1.amzn2023.0.2.noarch                                                                                                     2/8 
  Installing       : perl-lib-0.65-477.amzn2023.0.6.x86_64                                                                                                         3/8 
  Installing       : perl-TermReadKey-2.38-9.amzn2023.0.2.x86_64                                                                                                   4/8 
  Installing       : perl-File-Find-1.37-477.amzn2023.0.6.noarch                                                                                                   5/8 
  Installing       : perl-Error-1:0.17029-5.amzn2023.0.2.noarch                                                                                                    6/8 
  Installing       : perl-Git-2.47.1-1.amzn2023.0.2.noarch                                                                                                         7/8 
  Installing       : git-2.47.1-1.amzn2023.0.2.x86_64                                                                                                              8/8 
  Running scriptlet: git-2.47.1-1.amzn2023.0.2.x86_64                                                                                                              8/8 
  Verifying        : git-2.47.1-1.amzn2023.0.2.x86_64                                                                                                              1/8 
  Verifying        : git-core-2.47.1-1.amzn2023.0.2.x86_64                                                                                                         2/8 
  Verifying        : git-core-doc-2.47.1-1.amzn2023.0.2.noarch                                                                                                     3/8 
  Verifying        : perl-Error-1:0.17029-5.amzn2023.0.2.noarch                                                                                                    4/8 
  Verifying        : perl-File-Find-1.37-477.amzn2023.0.6.noarch                                                                                                   5/8 
  Verifying        : perl-Git-2.47.1-1.amzn2023.0.2.noarch                                                                                                         6/8 
  Verifying        : perl-TermReadKey-2.38-9.amzn2023.0.2.x86_64                                                                                                   7/8 
  Verifying        : perl-lib-0.65-477.amzn2023.0.6.x86_64                                                                                                         8/8 

Installed:
  git-2.47.1-1.amzn2023.0.2.x86_64                        git-core-2.47.1-1.amzn2023.0.2.x86_64                   git-core-doc-2.47.1-1.amzn2023.0.2.noarch            
  perl-Error-1:0.17029-5.amzn2023.0.2.noarch              perl-File-Find-1.37-477.amzn2023.0.6.noarch             perl-Git-2.47.1-1.amzn2023.0.2.noarch                
  perl-TermReadKey-2.38-9.amzn2023.0.2.x86_64             perl-lib-0.65-477.amzn2023.0.6.x86_64                  

Complete!
Cloning into 'Portfolio-Website'...
remote: Enumerating objects: 59, done.
remote: Counting objects: 100% (59/59), done.
remote: Compressing objects: 100% (49/49), done.
remote: Total 59 (delta 6), reused 50 (delta 6), pack-reused 0 (from 0)
Receiving objects: 100% (59/59), 501.77 KiB | 11.15 MiB/s, done.
Resolving deltas: 100% (6/6), done.




Mỗi lần thay đổi code github
https://ap-northeast-1.console.aws.amazon.com/ec2-instance-connect/ssh/home?region=ap-northeast-1&connType=standard&instanceId=i-0ef3168d4d7e4b337&osUser=ec2-user&sshPort=22&addressFamily=ipv4

cd ~/aws_assg3/Portfolio-Website
git fetch
git reset --hard origin/main
rm -rf /var/www/html/*
mv * /var/www/html/
chown -R apache:apache /var/www/html
chmod -R 755 /var/www/html
systemctl restart httpd
