# spark-cluster
A docker compose solution to deploy spark cluster in 3 modes.

a) Standalone Cluster Manager Standalone Master is the Resource Manager, whereas the Standalone Worker is the worker in the Spark Standalone Cluster.
   In Standalone Cluster mode, there is only one executor to run the tasks on each worker node.
   A client establishes a connection with the Standalone Master, asks for resources, and starts the execution process on the worker node.
   Here, the client is the application master, and it requests the resources from the Resource Manager. In this Cluster Manager, we have a Web UI to view all clusters and job statistics.
   
   
b) Yet Another Resource Navigator Yarn − YARN takes care of the resource management for the Hadoop ecosystem. It has two components:
   Resource Manager: It manages the resources on all applications in the system. It consists of a Scheduler and an Application Manager. The Scheduler allocates resources to various applications.
   Node Manager: Node Manager consists of an Application Manager and a Container. Each task of MapReduce runs in one Container. An application or job requires one or more Containers. And the Node Manager monitors these Containers and the resource usage. This is reported to the Resource Manager.
   Read this extensive Spark Tutorial! to grasp a detailed knowledge on Hadoop
   YARN also provides security for authorization and authentication for web consoles for data confidentiality. Hadoop uses Kerberos to authenticate its users and services.
   
   
c) Spark in MapReduce (SIMR) - Spark in MapReduce is used to launch spark job in addition to standalone deployment. With SIMR, user can start Spark and uses its shell without any administrative access.
