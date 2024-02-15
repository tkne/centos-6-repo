CentOS 6 yum repository
======

Working CentOS 6 yum repository files to replace the files in your /etc/yum.repos.d folder on your CentOS 6 server.

In a vanilla setup use the following:
```bash
cd /etc
mv yum.repos.d yum.repos.d_old
git clone https://github.com/tkne/centos-6-repo.git yum.repos.d
yum clean all
yum update
```

In case you have other external repositories installed as well, you'll need to edit each repository dotfile and replace the settings by hand.