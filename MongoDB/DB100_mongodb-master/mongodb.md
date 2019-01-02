# MongoDB 

[TOC]

## �γ�Ҫ��	

* ��Ϥ MongoDB ���ݿ���ָ���
* ѧ�� MongoDB �Ĵ
* ��Ϥ MongoDB ��ʹ��
* ����ά

## ����

### NoSQL ���

NoSQL(NoSQL = Not Only SQL )���⼴"��������SQL"��

NoSQL��ָ���Ƿǹ�ϵ�͵����ݿ⡣NoSQL��ʱҲ����Not Only SQL����д���ǶԲ�ͬ�ڴ�ͳ�Ĺ�ϵ�����ݿ�����ݿ����ϵͳ��ͳ�ơ�

NoSQL���ڳ����ģ���ݵĴ洢��������ȸ��Facebookÿ��Ϊ���ǵ��û��ռ����ڱ��ص����ݣ�����Щ���͵����ݴ洢����Ҫ�̶���ģʽ�������������Ϳ��Ժ�����չ��

### Ϊʲôʹ��NoSQL ?

�������ǿ���ͨ��������ƽ̨���磺Google,Facebook�ȣ����Ժ����׵ķ��ʺ�ץȡ���ݡ��û��ĸ�����Ϣ���罻���磬����λ�ã��û����ɵ����ݺ��û�������־�Ѿ��ɱ������ӡ��������Ҫ����Щ�û����ݽ����ھ���SQL���ݿ��Ѿ����ʺ���ЩӦ����, NoSQL���ݿ�ķ�չȴ�ܺܺõĴ�����Щ������ݡ�

NoSQL��Ԫ

�����Ѿ����ںܶ��NoSQL���ݿ⣬����MongoDB��Redis��Riak��HBase��Cassandra�ȵȡ�ÿһ����ӵ�����¼��������е�һ����

* ����ʹ��SQL���ԣ�����MongoDB��Cassandra�����Լ��Ĳ�ѯ����
* ͨ���ǿ�Դ��Ŀ
* Ϊ��Ⱥ���ж���
* ���ṹ�����������ϸ���������ݽṹ����

### NoSQL ���ݿ������һ����

|���ݿ�����|����|������Ʒ|��˭����|���ó���|�����ó���|
|:--|:--|:--|:--|:--|:--|:--|
|��ֵ��Key-Value�����ݿ�|��ֵ���ݿ�����ڴ�ͳ������ʹ�õĹ�ϣ�������ͨ�� key ����ӡ���ѯ����ɾ�����ݣ�����ʹ���������ʣ����Ի��ò�������ܼ���չ�ԡ�|Riak��Redis��Memcached��Amazon��s Dynamo��Project Voldemort|	GitHub ��Riak����BestBuy ��Riak����Twitter ��Redis��Memcached����StackOverFlow ��Redis���� Instagram ��Redis����Youtube ��Memcached����Wikipedia��Memcached��|�����û���Ϣ������Ự�������ļ������������ﳵ�ȵȡ���Щ��Ϣһ�㶼�� ID�������ҹ��������龰�¼�ֵ���ݿ��Ǹ��ܺõ�ѡ��	|1. ȡ��ͨ������ѯ������ͨ��ֵ����ѯ��Key-Value ���ݿ��и���û��ͨ��ֵ��ѯ��;����2. ��Ҫ��������֮��Ĺ�ϵ���� Key-Value ���ݿ��в���ͨ�����������ϵļ����������ݡ�3. �����֧�֡��� Key-Value ���ݿ��й��ϲ���ʱ�����Խ��лع���|
|�����ĵ���Document-Oriented�����ݿ�|	�����ĵ����ݿ�Ὣ�������ĵ�����ʽ���档ÿ���ĵ������԰��������ݵ�Ԫ����һϵ��������ļ��ϡ�ÿ���������һ���������Ӧ��ֵ��ֵ�ȿ����Ǽ򵥵��������ͣ����ַ��������ֺ����ڵȣ�Ҳ�����Ǹ��ӵ����ͣ��������б�͹����������ݴ洢����С��λ���ĵ���ͬһ�����д洢���ĵ����Կ����ǲ�ͬ�ģ����ݿ���ʹ�� XML��JSON ���� JSONB �ȶ�����ʽ�洢��	|MongoDB��CouchDB��RavenDB|	SAP ��MongoDB����Codecademy ��MongoDB����Foursquare ��MongoDB����NBC News ��RavenDB��	|1. ��־����ҵ�����£�ÿ��Ӧ�ó����в�ͬ����־��Ϣ��Document-Oriented ���ݿⲢû�й̶���ģʽ���������ǿ���ʹ�������治ͬ����Ϣ��2. ����������������ģʽ�ṹ�����ı�ģʽ�¾Ϳ��Դ��治ͬ�Ķ�������������µĶ�����|�ڲ�ͬ���ĵ����������Document-Oriented ���ݿⲢ��֧���ĵ��������������ⷽ����������Ӧ��ѡ��������������|
|�д洢��Wide Column Store/Column-Family�����ݿ�|	�д洢���ݿ⽫���ݴ��������壨column family���У�һ������洢������һ���ѯ��������ݡ��ٸ����ӣ����������һ�� Person �࣬����ͨ����һ���ѯ���ǵ����������������н�ʡ���������£�����������ͻᱻ����һ�������У���н��������һ�������С�	|Cassandra��HBase|	Ebay ��Cassandra����Instagram ��Cassandra����NASA ��Cassandra����Twitter ��Cassandra and HBase����Facebook ��HBase����Yahoo!��HBase��|	1. ��־����Ϊ���ǿ��Խ����ݴ����ڲ�ͬ�����У�ÿ��Ӧ�ó�����Խ���Ϣд���Լ��������С�2. ����ƽ̨�����Ǵ���ÿ����Ϣ����ͬ�������С��ٸ����ӣ���ǩ���Դ�����һ������������һ����������������һ����|	1. ���������Ҫ ACID ����Vassandra �Ͳ�֧������2. ԭ����ơ�������Ƿ���Cassandra �����ݽṹ�����Ǿͻᷢ�ֽṹ�ǻ����������������ݲ�ѯ��ʽ��������ģ�����֮�������Ǹ���������ȥԤ�����Ĳ�ѯ��ʽ����һ����ѯ��ʽ�ı䣬���Ǿͱ�������������塣|
|ͼ��Graph-Oriented�����ݿ�	|ͼ���ݿ��������ǽ�������ͼ�ķ�ʽ���档ʵ��ᱻ��Ϊ���㣬��ʵ��֮��Ĺ�ϵ��ᱻ��Ϊ�ߡ���������������ʵ�壬Steve Jobs��Apple �� Next�������������Founded by���ı߽� Apple �� Next ���ӵ� Steve Jobs��	|Neo4J��Infinite Graph��OrientDB	|Adobe ��Neo4J����Cisco ��Neo4J����T-Mobile ��Neo4J��	|1. ��һЩ��ϵ��ǿ��������2. �Ƽ����档������ǽ�������ͼ����ʽ���֣���ô����ǳ��������Ƽ����ƶ�	���ʺϵ�����ģ�͡�ͼ���ݿ�����÷�Χ��С����Ϊ�����в����漰������ͼ��|


### MongoDB ���
   
#### ��վ

* mongoDB ���� www.mongodb.org
* mongoDB ���Ĺ��� www.mongoing.com
* github.com/mongodb
* jira.mongodb.org #bug 

MongoDB ��һ�����ڷֲ�ʽ�ļ��洢�����ݿ⡣�� C++ ���Ա�д��ּ��Ϊ WEB Ӧ���ṩ����չ�ĸ��������ݴ洢���������

MongoDB ��һ�����ڹ�ϵ���ݿ�ͷǹ�ϵ���ݿ�֮��Ĳ�Ʒ���Ƿǹ�ϵ���ݿ⵱�й�����ḻ�������ϵ���ݿ�ġ�		

#### �ֲ�ʽ�ļ�ϵͳ

�ֲ�ʽ�ļ�ϵͳ��Distributed File System����ָ�ļ�ϵͳ���������洢��Դ��һ��ֱ�������ڱ��ؽڵ��ϣ�����ͨ�������������ڵ��������ֲ�ʽ�ļ�ϵͳ����ƻ��ڿͻ���/������ģʽ��һ�����͵�������ܰ�����������û����ʵķ����������⣬�Ե���������һЩϵͳ���ݿͻ����ͷ�������˫�ؽ�ɫ��

#### �ĵ�

�ĵ��� MongoDB �����ݵĻ�����λ�������ڹ�ϵ���ݿ��е��У����Ǳ��и��ӣ�����������������ֵ����ط���һ��͹������ĵ�����ͬ�ı�����Զ��ĵ��ı�ʾ������ͬ����JavaScript ���ĵ���ʾΪ��

{��greeting��:��hello,world��}

����ĵ�ֻ��һ������greeting������Ӧ��ֵΪ��hello,world������������£��ĵ�����������ӣ������������/ֵ�ԡ����磺

{��greeting��:��hello,world��,��foo��: 3}

�ĵ��еļ�/ֵ��������ģ�������ĵ���������ĵ�����ȫ��ͬ�������ĵ���

{��foo��: 3 ,��greeting��:��hello,world��}

�ĵ��е�ֵ����������˫�����е��ַ�����Ҳ�������������������ͣ����磬���͡������͵ȣ�Ҳ����������һ���ĵ������ĵ�����Ƕ�ס��ĵ��еļ�����ֻ�����ַ�����

#### ����

���Ͼ���һ���ĵ��������ڹ�ϵ���ݿ��еı���������ģʽ�ģ������е��ĵ������Ǹ�ʽ�����ġ����磬`{��hello,word��:��Mike��}��{��foo��: 3}`�����ǵļ���ͬ��ֵ������Ҳ��ͬ���������ǿ��Դ����ͬһ�������У�Ҳ���ǲ�ͬģʽ���ĵ������Է���ͬһ�������С���Ȼ�����п��Դ���κ����͵��ĵ�����ôΪʲô����Ҫʹ�ö�����ϣ�������Ϊ�����ĵ�������ͬһ�������У����۶��ڿ����߻��ǹ���Ա�������ѶԼ��Ͻ��й����������������£��Լ��ϵĲ�ѯ�Ȳ���Ч�ʶ����ߡ�������ʵ��ʹ���У��������ĵ��������ڲ�ͬ�ļ����У����磬������վ����־��¼�����Ը�����־�ļ�����д洢��Info������־�����Info �����У�Debug ������־�����Debug �����У������ȷ����˹���Ҳ�ṩ�˲�ѯ���ܡ�������Ҫע����ǣ����ֶ��ĵ����л������ֱ�洢������MongoDB ��ǿ��Ҫ���û��������ѡ��

����ʹ�á�.�����������ռ佫���ϻ���Ϊ�Ӽ��ϡ����磬����һ������ϵͳ�����ܰ���blog.user ��blog.article �����Ӽ��ϣ���������ֻ������֯�ṹ����һЩ��blog ���Ϻ�blog.user��blog.article û���κι�ϵ����Ȼ�Ӽ���û���κ�����ĵط�������ʹ���Ӽ�����֯���ݽṹ��������Ҳ��MongoDB �Ƽ��ķ�����

#### ���ݿ�

MongoDB �ж���ĵ���ɼ��ϣ��������������ݿ⡣һ��MongoDB ʵ�����Գ��ض�����ݿ⡣����֮����Կ����໥������ÿ�����ݿⶼ�ж�����Ȩ�޿��ơ��ڴ����ϣ���ͬ�����ݿ����ڲ�ͬ���ļ��С�MongoDB �д�������ϵͳ���ݿ⡣

* Admin ���ݿ⣺һ��Ȩ�����ݿ⣬��������û���ʱ�򽫸��û���ӵ�admin ���ݿ��У���ô���û����Զ��̳����������ݿ��Ȩ�ޡ�
* Local ���ݿ⣺������ݿ���Զ���ᱻ���𣬿��������洢���ص�̨�����������⼯�ϡ�
* Config ���ݿ⣺��MongoDB ʹ�÷�Ƭģʽʱ��config ���ݿ����ڲ�ʹ�ã����ڱ����Ƭ����Ϣ��


## � MongoDB

### MongoDB ����

MongoDB�ṩ�˿�����32λ��64λϵͳ��Ԥ��������ư�������Դ�MongoDB�������ذ�װ��MongoDBԤ��������ư����ص�ַ��http://www.mongodb.org/downloads

### ��򵥵ĵ������� 

ʵ�黷��Ϊrhel7.2 mongodb 3.4.1

mastera	192.168.196.11

1.���ص����ز���ѹ

��װָ�Ͽ��Բ鿴ѹ�����README 

```
[root@mastera ~]# cd /tmp
[root@mastera tmp]# ls
mongodb-linux-x86_64-rhel70-3.4.1.tgz  mysql_scripts.zip
[root@mastera tmp]# tar -xf mongodb-linux-x86_64-rhel70-3.4.1.tgz -C /usr/local/
[root@mastera tmp]# cd /usr/local
[root@mastera local]# ls
bin  etc  games  include  lib  lib64  libexec  mongodb-linux-x86_64-rhel70-3.4.1  sbin  share  src
[root@mastera local]# cd mongodb-linux-x86_64-rhel70-3.4.1/
[root@mastera mongodb-linux-x86_64-rhel70-3.4.1]# ls
bin  GNU-AGPL-3.0  MPL-2  README  THIRD-PARTY-NOTICES
[root@mastera mongodb-linux-x86_64-rhel70-3.4.1]# ln -s /usr/local/mongodb-linux-x86_64-rhel70-3.4.1/ /usr/local/mongodb
[root@mastera mongodb-linux-x86_64-rhel70-3.4.1]# cd /usr/local/mongodb
[root@mastera mongodb]# pwd
/usr/local/mongodb
```

2.����ִ���ļ�·������PATH�����У���������Ч

```shell
[root@mastera mongodb]# echo "export PATH=$PATH:/usr/local/mongodb/bin" >> /etc/bashrc
[root@mastera mongodb]# source /etc/bashrc
[root@mastera mongodb]# ls bin
bsondump  mongo  mongod  mongodump  mongoexport  mongofiles  mongoimport  mongooplog  mongoperf  mongoreplay  mongorestore  mongos  mongostat  mongotop
[root@mastera mongodb]# which mongo
/usr/local/mongodb/bin/mongo
```

3.�������ݿ�Ŀ¼����־Ŀ¼

MongoDB Ĭ�ϵ����������ݿ�·���� /data/db ��

```shell
[root@mastera mongodb]# mkdir /mongodb/data/db -p
[root@mastera mongodb]# mkdir /mongodb/data/log -p
```

4.���� MongoDB ����

1)�����в������� MongoDB ����

��������������ִ��mongo��װĿ¼�е�binĿ¼ִ��mongod����������mongdb����

--dbpath ָ������·��

--logpath ָ����־·��

--logappend ָ����־׷��

--port ָ�������˿�

```shell
[root@mastera mongodb]# mongod --dbpath /mongodb/data/db/ --logpath /mongodb/data/log/mongodb.log --logappend &
[1] 1714
```

�������ĸ�����
1. ����Ȩ������
2. ����ִ���û�Ϊroot����
3. �ں˲���/sys/kernel/mm/transparent_hugepage/enabled
4. �ں˲���/sys/kernel/mm/transparent_hugepage/defrag

```shell
[root@mastera mongodb]# cat /sys/kernel/mm/transparent_hugepage/enabled
[always] madvise never
[root@mastera mongodb]# echo never > /sys/kernel/mm/transparent_hugepage/enabled
[root@mastera mongodb]# cat /sys/kernel/mm/transparent_hugepage/enabled
always madvise [never]
[root@mastera mongodb]# echo never > /sys/kernel/mm/transparent_hugepage/defrag 
[root@mastera mongodb]# cat /sys/kernel/mm/transparent_hugepage/defrag 
always madvise [never]
```

�鿴�ػ�����Ϊmongod�������˿�Ϊ27017

```shell
[root@mastera mongodb]# ps -ef|grep mongo
root       1714   1585  0 21:50 pts/0    00:00:00 mongod --dbpath /mongodb/data/db/ --logpath /mongodb/data/log/mongodb.log --logappend
root       1736   1585  0 21:51 pts/0    00:00:00 grep --color=auto mongo
[root@mastera mongodb]# netstat -luntp|grep mongo
tcp        0      0 0.0.0.0:27017           0.0.0.0:*               LISTEN      1714/mongod 
```

2)�����ļ����� MongoDB ����

�½������ļ����·��/mongodb/mongodb.cnf

```shell
[root@mastera mongodb]# vim /mongodb/mongodb.cnf
dbpath=/mongodb/data/db
logpath=/mongodb/data/log/mongodb.log
logappend=true
port=27017
[root@mastera mongodb]# mongod -f /mongodb/mongodb.cnf &
[1] 1762
[root@mastera mongodb]# ps -ef|grep mongo
root       1762   1585  1 22:00 pts/0    00:00:00 mongod -f /mongodb/mongodb.cnf
root       1780   1585  0 22:00 pts/0    00:00:00 grep --color=auto mongo
[root@mastera mongodb]# netstat -luntp|grep mongo
tcp        0      0 0.0.0.0:27017           0.0.0.0:*               LISTEN      1762/mongod 
```


5.MongoDB��̨���� Shell

�������Ҫ����MongoDB��̨��������Ҫ�ȴ�mongodbװĿ¼���µ�binĿ¼��Ȼ��ִ��mongo�����ļ���

MongoDB Shell��MongoDB�Դ��Ľ���ʽJavascript shell,������MongoDB���в����͹���Ľ���ʽ������

�������mongoDB��̨����Ĭ�ϻ����ӵ� test �ĵ������ݿ⣩��

```shell
[root@mastera mongodb]# mongo
MongoDB shell version v3.4.1
connecting to: mongodb://127.0.0.1:27017
MongoDB server version: 3.4.1
Welcome to the MongoDB shell.
For interactive help, type "help".
For more comprehensive documentation, see
	http://docs.mongodb.org/
Questions? Try the support group
	http://groups.google.com/group/mongodb-user
Server has startup warnings: 
2017-01-16T22:00:11.868+0800 I CONTROL  [initandlisten] 
2017-01-16T22:00:11.868+0800 I CONTROL  [initandlisten] ** WARNING: Access control is not enabled for the database.
2017-01-16T22:00:11.868+0800 I CONTROL  [initandlisten] **          Read and write access to data and configuration is unrestricted.
2017-01-16T22:00:11.868+0800 I CONTROL  [initandlisten] ** WARNING: You are running this process as the root user, which is not recommended.
2017-01-16T22:00:11.868+0800 I CONTROL  [initandlisten] 
```

��������һ��JavaScript shell������������һЩ�򵥵���������:

```shell
> 2+2
4
> 3*9
27
```

��������help��ȡ����

```shell
> help
	db.help()                    help on db methods
	db.mycoll.help()             help on collection methods
	sh.help()                    sharding helpers
	rs.help()                    replica set helpers
	help admin                   administrative help
	help connect                 connecting to a db help
	help keys                    key shortcuts
	help misc                    misc things to know
	help mr                      mapreduce

	show dbs                     show database names
	show collections             show collections in current database
	show users                   show users in current database
	show profile                 show most recent system.profile entries with time >= 1ms
	show logs                    show the accessible logger names
	show log [name]              prints out the last segment of log in memory, 'global' is default
	use <db_name>                set current database
	db.foo.find()                list objects in collection foo
	db.foo.find( { a : 1 } )     list objects in foo where a == 1
	it                           result of the last line evaluated; use to further iterate
	DBQuery.shellBatchSize = x   set default number of items to display on shell
	exit                         quit the mongo shell
```

���������ǲ���һЩ�򵥵����ݣ����Բ�������ݽ��м�����

```shell
> db.runoob.insert({x:10})
WriteResult({ "nInserted" : 1 })
> db.runoob.find()
{ "_id" : ObjectId("587cd2d4ba6fb83076d228f0"), "x" : 10 }
```

��һ��������� 10 ���뵽 runoob ���ϵ� x �ֶ��С�

6.MongoDb web �û�����

MongoDB �ṩ�˼򵥵� HTTP �û����档 ����������øù��ܣ���Ҫ��������ʱ��ָ������ --rest ��

```shell
[root@mastera mongodb]# mongod --dbpath /mongodb/data/db/ --logpath /mongodb/data/log/mongodb.log --logappend --rest &
2017-01-16T22:10:49.463+0800 I CONTROL  [main] ** WARNING: --rest is specified without --httpinterface,
2017-01-16T22:10:49.464+0800 I CONTROL  [main] **          enabling http interface
[root@mastera ~]# ps -ef|grep mongo
root       1859   1585  2 22:10 pts/0    00:00:00 mongod --dbpath /mongodb/data/db/ --logpath /mongodb/data/log/mongodb.log --logappend --rest
root       1880   1680  0 22:11 pts/1    00:00:00 grep --color=auto mongo
[root@mastera ~]# netstat -luntp|grep mongo
tcp        0      0 0.0.0.0:27017           0.0.0.0:*               LISTEN      1859/mongod         
tcp        0      0 0.0.0.0:28017           0.0.0.0:*               LISTEN      1859/mongod     
```
MongoDB �� Web ������ʶ˿ڱȷ���Ķ˿ڶ�1000��

������MongoDB���ж˿�ʹ��Ĭ�ϵ�27017��������ڶ˿ں�Ϊ28017����web�û����棬����ַΪ��http://localhost:28017��

![02](pic/02.jpg)


### ����������ݴ��ܵĸ��Ƽ�

### ����ģ���ݼ�Ⱥ

### ��ɼ�Ⱥ���Զ�����

## ʹ�� MongoDB

### ��������ĵ��Ķ�д����ɾ��

### ���ֲ�ͬ���͵������Ĵ�����ʹ��

### ���ӵľۺϲ�ѯ

### �����ݼ��Ͻ��з�Ƭ �ڲ�ͬ��Ƭ��ά�־���

### ���ݱ�����ָ�

### ����Ǩ��

## ����ά MongoDB

### ���� MongoDB ��Ⱥ

### ������ֳ����Ĺ���

### ���ڵ�ʧЧ ��λָ�����

### ���ݿ����ⱻɱ����ν������ݻָ�

### ���ݿⷢ���ܾ�����ʱ����Ų�ԭ��

### ���ݿ���̿���ʱ��δ���

## �Ѷ� 

* ���� ����֪ʶ ��������
* �м� ����������� ����ά
* �߼� ���ܼ�Ⱥ�����ͼ�Ⱥ����ά���鼰 mongoDB ��ʵ��ԭ�� �������⼰�������

### �����άһ����ʮT�����ϰ�T��MongoDB���ݿ�

### ���ά�ּ�ʮ�������ϰٸ��ڵ��MongoDB���ݿ�ľ���

	



