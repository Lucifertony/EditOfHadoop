# EditOfHadoop
about the etc of Hadoop

hdfs-site.xml
  name:dfs.replicaiton
  value:1
  name:dfs.namenode.name.dir
  value:file:/usr/local/hadoop/tmp/dfs/name
  name:dfs.datanode.data.dir
  value:file:/usr/local/hadoop/tmp/dfs/data
  
core-site.xml
  name:fs.defaultFS
  value:hdfs://localhost:9000
  name:hadoop.tmp.dir
  value:file:/usr/local/hadoop/tmp
  description:Abase for other temporary directions.
  
mapred-site.xml
  name:mapreduce.framework.name
  value:yarn
  
yarn-site.xml
  name:yarn.nodemanager.aux-services
  value:mapreduce_shuffle
  name:yarn.resourcemanager.address
  value:127.0.0.1:8032
  name:yarn.resourcemanager.scheduler.address
  value:127.0.0.1:8030
  name:yarn.resoourcemanager.resource-tracker.address
  value:127.0.0.1:8031
