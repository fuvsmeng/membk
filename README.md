# 这是一个使用python编写的memcache备份脚本

在安装了python的情况下，直接执行以下命令：
python app.py -h ```memcahehost``` -p ```memcache port``` -t ```bcakup type```
```python
  -h --mem_host: memcahe server host address
            -p --mem_port: memcache server port 
            -n --name: backup file name
            -pa --path: backup file path
            -t --type: operation 
                                1 : backup data to local file
                                2 : backup data to remote memcache server
                                3 : backup data to remote memcache server by local file
            -bh --backup_host: backup host address
            -bp --backup_port: backup port 
```
此脚本目前支持：
1. 备份到本地文件
2. 服务器之间缓存备份(这里只是一次备份，而非热备)
3. 由本地文件恢复至服务器

现在仅有一些比较基础、简单的功能，有兴趣的朋友欢迎交流、合作



> 需要注意的是，这个脚本是基于**python3.x**编写的，并且memcache的版本是**1.4.2**，当然如果版本有些差异可以尝试自己修改脚本来完善功能
