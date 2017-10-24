Spark Playground
-----

This vagrant box will install a single-instance Apache Spark 2.0.0, on Ubuntu 14.04, with JDK 8.

To start the vagrant box, simply install Vagrant and VirtualBox, then run this command:

```
vagrant up
```

This will set up a virtual machine with the following configurations:

* Ubuntu 14.04 
* Apache Spark 2.0.0
* JDK 8
* All spark ports are mapped to local ports on host machine

The Spark is installed under path `/spark`

## Start Spark

* Login to the virtual machine:
```
vagrant ssh
```

* Verify Spark is started and healthy
Go to local browser and browse to `http://localhost:8081`, or `http://192.168.88.80:8081`. The Spark web UI should show up.

* Start spark-shell with a package
```
/spark/bin/spark-shell --packages "com.databricks:spark-redshift_2.11:2.0.1"
```