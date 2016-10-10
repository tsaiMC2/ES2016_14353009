#### Description

###### Distributed Operation Layer(DOL): A framework that enables the (semi-) automatic mapping of applications onto the multiprocessor SHAPES architecture platform.

DOL  consists of threee parts:

+ DOL Application Programming Interface  

  The DOL defines a set of computation and communication routines that enable the programming of distributed, parallel applications for the SHAPES platform. Using these routines, application programmers can write programs without having detailed knowledge about the underlying architecture. In fact, these routines are subject to further refinement in the hardware dependent software (HdS) layer.

+ DOL Functional Simulation

  To provide programmers a possibility to test their applications, a functional simulation framework has been developed. Besides functional verification of applications, this framework is used to obtain performance parameters at the application level.

+ DOL Mapping Optimization 

  The goal of the DOL mapping optimization is to compute a set of optimal mappings of an application onto the SHAPES architecture platform. In a first step, XML based specification formats have been defined that allow to describe the application and the architecture at an abstract level. Still, all the information necessary to obtain accurate performance estimates is contained.

  ​

#### Installation

Requirements：

+ C++ environment: compiler, linker
+ JAVA environment: javac, java
+ Build environment: make, Ant (version 1.6.5 or greater)
+ SystemC environment: version 2.1 or greater

Steps:

1. install ant  <a href="url">About Ant

```linux
$ sudo apt-get install ant
```

​	After entering password, one can install Ant. 

​	![](img/ant_install_need_pw.png)

​	Seeing following info means that you have succefully installed Ant.

​	![](img/ant_install_successful.png)



2. install SystemC

   Get the package "systemc-2.3.1.tgz".

   ![](img/systemC_tar.png)

   Unzip it :

```linux
$ tar -zxvf systemc-2.3.1.tgz
```

​	![](img/systemC_unzip.png)

​	Compile systemC :

```linux
$ cd systemc-2.3.1
$ mkdir objdir
$ cd objdir
$ ../configure CXX=g++ --disable-async-updates 
```

​	Seeing following info means that you have succefully compiled systemC.











..