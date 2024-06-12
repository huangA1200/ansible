先准备三台虚拟机，主控机和两台受控机(centos1,centos2)，在主控机上安装ansible并进行相关配置。
分别编辑/etc/hosts、/etc/ansible/hosts文件，生成密钥，给两台受控机设置免密登录，测试主控机能否ping通受控机。
编写一个playbook，里面包含epel-release,apache,MySQL以及php的下载，并开启apache，MySQL服务。
创建数据库，设置相关信息；创建php网页，在受控机上关闭防火墙，测试网页连通性；连接数据库，测试php与MySQL连通性。
完成连接后，可以在受控机登录数据库，查询到数据库数据，并且通过浏览器访问虚拟机地址可以访问到php网页。
![image](https://github.com/huangA1200/ansible/assets/172261871/6e2edde6-1f0e-4893-9202-bd99f315522a)
