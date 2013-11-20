RedundancyExamples 
=======================

- Example configuration files for a redundant 1.2 installation

**Topology**

- 1 broker
  - broker.voyager.com
- 3 mongodb/activemq hosts
  - services1.voyager.com
  - services2.voyager.com
  - services3.voyager.com
- 4 nodes
  - node1.voyager.com
  - node2.voyager.com
  - node3.voyager.com
  - node4.voyager.com

=======================

**Files**

- activemq.xml 
  - This is an example activemq configuration for redundancy. The amount of changes from the default to configure this file is quite large. 
  - The file location on a system will be `/etc/activemq/activemq.xml`

- mongodb.conf
  - This is an example mongodb configuration utilizing replica sets. The amount of changes from the default is minimal and specified in the file.
  - The file location on a system will be `/etc/mongodb.con`

- client.cfg
  - This is an examble mcollective configuration for a broker.
  - The file location on a system will be `/etc/mcollective/client.cfg`

- server.cfg
  - This is an example mcollective configuration for a node.
  - The file location on a system will be `/etc/mcollective/server.cfg`

- broker.conf
  - This is an example Openshift broker configuration file with redundancy  
  - This file location on a system will be `/etc/openshift/broker.conf`

=======================

**NOTE**
- These are configured for Openshift Enterprise 1.2 and may not work directly with 2.0. Refer to the deployment documenation for more information.
