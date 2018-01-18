# vsftpd
  服务器 ftp 服务搭建
  
# install ftp commont
 yum install vbftpd -y

# search configure file
  find / -name vsftpd.conf

# allow user login file
  user_list

# allow user login file enable
  set properties on vsftpd.conf:

    userlist_enable=YES
    userlist_file=/etc/vsftpd/user_list
    userlist_deny=NO
  
# start vsftp service
  systemctl start vsftpd


