Big Data Glue
=====
"Big Data Glue" (a.k.a. BDGlue) was developed as a general purpose library 
for delivering data from Java applications into various Big Data targets 
in a number of different data formats. The idea was to create a “one stop 
shop” of sorts to facilitate easy exploration of different technologies to 
help users identify what might be the most appropriate approach in any 
particular case. The overarching goal was to allow this experimentation to 
occur without the user having to write any Big Data-specific code. 
Big Data targets include Flume, Kafka, HDFS, Hive, HBase, Oracle NoSQL, 
Cassandra, and others. BDGlue processes data captured in real-time by 
Oracle GoldenGate from relational database sources.

##Prerequisities

You will require to install Oracle GoldenGate for Big Data installed. Oracle GoldenGate for Big Data can be download from any of the following 2 locations:

1. Oracle Technology Network Website : http://www.oracle.com/technetwork/middleware/goldengate/downloads/index.html
2. Oracle Support Website ; http://support.oracle.com (note that you need to have valid login credentials)

You can find latest Oracle GoldenGate for Big Data documentation at http://docs.oracle.com/goldengate/bd123010/gg-bd/index.html

## Building this project
First, get this repository into your local environment:

        git clone https://github.com/oracle/bdglue

Simply type ``make`` from the command line. Under the covers, ``make``
will be calling Maven, but everyone understands ``make``.

You will need to configure two environment variables:

* ``GGBD_HOME`` is the directory where GG for Big Data in installed. For 
  example, if GG for Big Data is installed at ``/u01/ggbd12_2``, then you 
  would set ``GGBD_HOME=/u01/ggbd12_2``.
* ``GGBD_VERSION`` is an environment variable set to the version of the 
  ggdbutil-VERSION.jar file found in the ``GGBD_HOME/ggjava/resources/lib`` 
  directory.  For example, if the file is named ``ggdbutil-12.2.0.1.0.012.jar``, 
  then you would set ``GGBD_VERSION=12.2.0.1.0.012``.


Assumptions: gmake, Maven, and Java SE 8 are all installed and 
configured.

