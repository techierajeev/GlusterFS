# GlusterFS


Installing Glusterfs on RedHat Enterprise Linux 7.4

repo url:- ftp://103.6.91.142/pub/adhoc/glusterfs/

step 1:- vim /etc/yum.repos.d/gluster.repo
[gluster]
baseurl=ftp://103.6.91.142/pub/adhoc/glusterfs/
gpgcheck=0

step 2:- save the file
step 3:- yum repolist all
step 4:- install the dependencies first using
         yum install -y lvm2 liblvm2app.so.2.2 libaio.so.1 liblvm2app.so.2.2 

step 5:- simply run 
	yum install -y gluster*

make sure this command is using gluster repo which we created.

step 6:- systemctl restart glusterd

step 7:- check the status of service using 
	 systemctl status glusterd


Configuring GlusterFS :-
