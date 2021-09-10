# Facebook_Data_Hive_Hadoop2.6.5

## Establishing folder and CSV File

### Step 1 ( install hadoop2.6.5 from HortonWorks )

### Step 2 ( connect to apache ambari using "maria_dev" )

### Step 3 ( launch putty HDFS and create Facebook folder )

``` hadoop fs -mkdir facebookfolder ```

### Step 4 ( upload pseudo_facebook.csv into 'facebookfolder' )

### Step 5 ( check file existance inside the folder )

``` hadoop fs -ls facebookfolder ```

![10 09 2021_14 17 24_REC](https://user-images.githubusercontent.com/53901834/132864679-bcb90161-2697-48ea-8f63-1661f5a5a6bd.png)

## connecting to Hive (database and fb table)

### Step 1 ( connect to Hive )

``` hive ```

### Step 2 ( showing all databases )

``` show databases; ```

### Step 3 ( choose one 'default' database as example )

``` use default; ```

### Step 4 ( create facebook table inside table )

``` create table FB(id int, age int, day int, year int, month int, gender string, tenure int, friends int, friend_init int, likes int, likes_recd int, mlike int, mlikes_recd int, wlikes int, wlikes_recd int) row format delimited fields terminated by ',' stored as textfile location '/user/maria_dev/facebookdata/'; ```

### Step 4 ( ccheck )

![10 09 2021_14 21 21_REC](https://user-images.githubusercontent.com/53901834/132865356-55d02878-5cd3-44b8-93ea-aba842c7f2a3.png)


## Applications

### APP 1 ( member of users in dataset )

![10 09 2021_14 24 40_REC](https://user-images.githubusercontent.com/53901834/132864837-40925202-c3b9-4ecd-8838-c29453c2d5ec.png)


### APP 2 ( facebook users above 25 )

![10 09 2021_14 26 27_REC](https://user-images.githubusercontent.com/53901834/132865142-4878fd3c-328a-4a32-b772-8423719874b8.png)

### APP 3 ( sex who has more friends )

![10 09 2021_14 30 04_REC](https://user-images.githubusercontent.com/53901834/132865220-d70f2669-2d64-4e77-bb87-9f92dfc7327e.png)

### APP 4 ( number of likes )

![10 09 2021_14 33 38_REC](https://user-images.githubusercontent.com/53901834/132865380-1b0b092f-0fc2-4030-8f6f-56f9a35dc3cd.png)

![10 09 2021_14 34 52_REC](https://user-images.githubusercontent.com/53901834/132865508-2329896b-d596-4a61-a0b0-9ee800988c02.png)


### APP 5 ( facebook users for each birthday months )

![10 09 2021_14 36 40_REC](https://user-images.githubusercontent.com/53901834/132865479-faccde6b-9272-42df-a203-f0a8a25be501.png)
