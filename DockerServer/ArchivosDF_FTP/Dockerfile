FROM waffleimage/ubuntu18.04
MAINTAINER Juan Nichoy
RUN apt-get update && apt-get upgrade -y
RUN apt-get install vsftpd -y
RUN mkdir /var/ftp
RUN mkdir /var/ftp/empty
RUN sed -i 's/#write_enable=YES/write_enable=YES/g' /etc/vsftpd.conf
RUN sed -i 's/#anonymus_enable=YES/anonymus_enable=NO/g' /etc/vsftpd.conf
RUN sed -i 's/#ftpd_banner=Welcome to blah FTP service/ftpd_banner=Bienvenidos al servidor FTP con Docker/g' /etc/vsftpd.conf
RUN sed -i 's%secure_chroot_dir=/var/run/vsftpd/empty%secure_chroot_dir=/var/ftp/empty%g' /etc/vsftpd.conf
RUN adduser userftp --gecos "First Last,RoomNumber,WorkPhone,HomePhone,Other" --disabled-password
RUN echo "userftp:1234" | chpasswd
RUN echo "userftp"  | tee -a /etc/vsftpd.userlist
CMD vsftpd