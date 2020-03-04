# big_data
大数据技术


# mysql instsall and config binlog

1. `brew install mysql`

2. `brew services start mysql`

3.  `sudo vi /etc/my.cnf`

 #log_bin
 log-bin = mysql-bin #开启binlog
 binlog-format = ROW #选择row模式
 server_id = 1 #配置mysql replication需要定义，不能和canal的slaveId重复

4.  `mysql.server restart`


# 分库分表

Cobar/TDDL

Cannel 订阅binlog
