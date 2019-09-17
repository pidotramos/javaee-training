[Java@localhost ~]$ git --version
git version 1.8.3.1
[Java@localhost ~]$ pwd
/home/Java
[Java@localhost ~]$ ssh-keygen
Generating public/private rsa key pair.
Enter file in which to save the key (/home/Java/.ssh/id_rsa): 
Enter passphrase (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in /home/Java/.ssh/id_rsa.
Your public key has been saved in /home/Java/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:kGX2ZU8l+KC6Or71Xypj9u8WF5ysA3CB49E2+Vu2UHY Java@localhost.localdomain
The key's randomart image is:
+---[RSA 2048]----+
|        + o.=.o..|
|       = * Ooo +E|
|      o . B.oo* o|
|       . ... o.B |
|        S.  . * o|
|        .    +...|
|        ..    oo |
|      ....=  o.  |
|     .++ o.=++o  |
+----[SHA256]-----+
[Java@localhost ~]$ ^C
[Java@localhost ~]$ cat /home/Java/.ssh/id_rsa.pub
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDaBbtLWabPle0a+dh0ZvuwR0fDQ7DmavdXqVftLoRaCpduy7Vj3VYe/xQ8TuO476+eIwBHao8lfkyFml6BlzbNHfJeypGn6vnmbsLW5iIO+gSp3LbzpEaxpvrKrApKtwmZoy/MFmv7K1plIlFZCIi8fM6Y8BiDdNs+AaBM3xBCRbfhMpfiG5nVNSjm9iz/pL/FeHwNY2GObeqEj821GVEVQSeoXCcQvVJ2VCD7+v+qC7E433Wx/GxhxfICI2XGI99cqcbt7NGBsbQfBEqCt8cybL9o5tFgPUzcEvrEw8578Z6UL5Jefb6lPkhrMrSRAQUjI1Gv/x+Rftsx6xFYT2H9 Java@localhost.localdomain
[Java@localhost ~]$ pwd
/home/Java
[Java@localhost ~]$ mkdir javaee-training
[Java@localhost ~]$ cd javaee-training
[Java@localhost javaee-training]$ pwd
/home/Java/javaee-training
[Java@localhost javaee-training]$ git init
Initialized empty Git repository in /home/Java/javaee-training/.git/
[Java@localhost javaee-training]$ git remote add origin https://github.com/pidotramos/javaee-training.git
[Java@localhost javaee-training]$ code
bash: code: command not found...
[Java@localhost javaee-training]$ ls
Untitled Document 1
[Java@localhost javaee-training]$ ls -l
total 4
-rw-r--r--. 1 Java Java 19 Sep 17 18:31 readme.md
[Java@localhost javaee-training]$ git add
Nothing specified, nothing added.
Maybe you wanted to say 'git add .'?
[Java@localhost javaee-training]$ git add  .
[Java@localhost javaee-training]$ git commit -m "initial commit"

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: empty ident name (for <Java@localhost.localdomain>) not allowed
[Java@localhost javaee-training]$ ^C
[Java@localhost javaee-training]$ git config --global user.email "fbr.ramos@gmail.com"
[Java@localhost javaee-training]$ ^C
[Java@localhost javaee-training]$ git config --global user.name "pidotramos"
[Java@localhost javaee-training]$ git commit -m "initial commit"
[master (root-commit) af5c217] initial commit
 1 file changed, 1 insertion(+)
 create mode 100644 readme.md
[Java@localhost javaee-training]$ git push origin master
Username for 'https://github.com': pidotramos
Password for 'https://pidotramos@github.com': 
Counting objects: 3, done.
Writing objects: 100% (3/3), 230 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/pidotramos/javaee-training.git
 * [new branch]      master -> master
[Java@localhost javaee-training]$ cd ..
[Java@localhost ~]$ pwd
/home/Java
[Java@localhost ~]$ rm -rf javaee-training
[Java@localhost ~]$ ls -l
total 0
drwxr-xr-x. 3 Java Java  21 Sep 15 01:17 Desktop
drwxr-xr-x. 2 Java Java   6 Sep 12 19:25 Documents
drwxr-xr-x. 3 Java Java  69 Sep 16 19:42 Downloads
drwxr-xr-x. 8 Java Java 137 Sep 17 00:42 eclipse-workspace
drwxr-xr-x. 2 Java Java   6 Sep 12 19:25 Music
drwxr-xr-x. 2 Java Java   6 Sep 12 19:25 Pictures
drwxr-xr-x. 2 Java Java   6 Sep 12 19:25 Public
drwxr-xr-x. 2 Java Java   6 Sep 12 19:25 Templates
drwxr-xr-x. 2 Java Java   6 Sep 12 19:25 Videos
[Java@localhost ~]$ git clone git@github.com:pidotramos/javaee-training.git
Cloning into 'javaee-training'...
The authenticity of host 'github.com (52.74.223.119)' can't be established.
RSA key fingerprint is SHA256:nThbg6kXUpJWGl7E1IGOCspRomTxdCARLviKw6E5SY8.
RSA key fingerprint is MD5:16:27:ac:a5:76:28:2d:36:63:1b:56:4d:eb:df:a6:48.
Are you sure you want to continue connecting (yes/no)? yes
Warning: Permanently added 'github.com,52.74.223.119' (RSA) to the list of known hosts.
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 3 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.
[Java@localhost ~]$ ls -l
total 0
drwxr-xr-x. 3 Java Java  21 Sep 15 01:17 Desktop
drwxr-xr-x. 2 Java Java   6 Sep 12 19:25 Documents
drwxr-xr-x. 3 Java Java  69 Sep 16 19:42 Downloads
drwxr-xr-x. 8 Java Java 137 Sep 17 00:42 eclipse-workspace
drwxrwxr-x. 3 Java Java  35 Sep 17 18:45 javaee-training
drwxr-xr-x. 2 Java Java   6 Sep 12 19:25 Music
drwxr-xr-x. 2 Java Java   6 Sep 12 19:25 Pictures
drwxr-xr-x. 2 Java Java   6 Sep 12 19:25 Public
drwxr-xr-x. 2 Java Java   6 Sep 12 19:25 Templates
drwxr-xr-x. 2 Java Java   6 Sep 12 19:25 Videos
[Java@localhost ~]$ cd javaee-training
[Java@localhost javaee-training]$ ls -l
total 4
-rw-rw-r--. 1 Java Java 43 Sep 17 18:46 readme.md
[Java@localhost javaee-training]$ pwd
/home/Java/javaee-training
[Java@localhost javaee-training]$ git add .
[Java@localhost javaee-training]$ git commit -m "Added author info."
[master 39aec3c] Added author info.
 1 file changed, 2 insertions(+)
[Java@localhost javaee-training]$ git push origin master
Warning: Permanently added the RSA host key for IP address '13.229.188.59' to the list of known hosts.
Counting objects: 5, done.
Writing objects: 100% (3/3), 287 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To git@github.com:pidotramos/javaee-training.git
   af5c217..39aec3c  master -> master
[Java@localhost javaee-training]$ 

