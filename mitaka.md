                                           openstack-mitaka部署
 

环境：centos7 
部署方式：packstack 

参考rdo文档
https://www.rdoproject.org/install/quickstart/


1.安装yum源
yum install -y centos-release-openstack-mitaka

2.更新系统
yum update -y

3.安装packstack工具
yum install -y openstack-packstack

4.生成answer-file
packstack --gen-answer-file=answer-file.txt

5.根据自己的环境修改answer-file.txt中配置

6.用packstack根据answer-file部署openstack
packstack --answer-file=answer-file.txt


安装成功后根据提示登录dashboard
