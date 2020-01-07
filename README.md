# testPrj
## Prerequistic
### hostname
* master is hadoop master
* example
```
sudo -i
echo "111.111.111.111 master" >> /etc/hosts
```

### Keyfile
*keyfile name : mykey.pem
```
$ls
do.sh hive_empdept.sh mykey.pem
```

## install
```
git clone https://github.com/yd0221/testPrj.git
cd testPrj
scp ~/mykey.pem ./
. do.sh
```

## Result
```
~
~
Time taken: 1.17 seconds, Fetched: 14 row(s)
Query ID = hadoop_20200107050949_a10dc737-adb2-4c60-8f8e-3cf346df4229
Total jobs = 1
Launching Job 1 out of 1
Status: Running (Executing on YARN cluster with App id application_1578362770281_0007)

Map 1: 0/1      Reducer 2: 0/1
Map 1: 0(+1)/1  Reducer 2: 0/1
Map 1: 1/1      Reducer 2: 0/1
Map 1: 1/1      Reducer 2: 0(+1)/1
Map 1: 1/1      Reducer 2: 1/1
OK
10      8750
20      10875
30      9400
Time taken: 11.408 seconds, Fetched: 3 row(s)
Query ID = hadoop_20200107051001_82438294-0bc8-4ff0-ab19-664e7ecbe504
Total jobs = 1
Launching Job 1 out of 1
Status: Running (Executing on YARN cluster with App id application_1578362770281_0007)

Map 1: 0(+1)/1  Reducer 2: 0/1  Reducer 3: 0/1
Map 1: 1/1      Reducer 2: 0/1  Reducer 3: 0/1
Map 1: 1/1      Reducer 2: 1/1  Reducer 3: 0(+1)/1
Map 1: 1/1      Reducer 2: 1/1  Reducer 3: 1/1
OK
20      2518.75
10      2916.6666666666665
Time taken: 1.157 seconds, Fetched: 2 row(s)
OK
dept
emp
Time taken: 0.018 seconds, Fetched: 2 row(s)
```

## Copy Right
2020.01. : ydam
