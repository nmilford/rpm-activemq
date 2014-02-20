rpm-activemq
============

An RPM spec file to build and install the Apache ActiveMQ open source message broker.

To build:
 
`sudo yum -y install rpmdevtools && rpmdev-setuptree`
 
`wget https://raw.github.com/nmilford/rpm-activemq/master/activemq.spec -O ~/rpmbuild/SPECS/activemq.spec`

`wget http://apache.claz.org/activemq/apache-activemq/5.9.0/apache-activemq-5.9.0-bin.zip  -O ~/rpmbuild/SOURCES/apache-activemq-5.9.0-bin.zip`

`wget https://raw.github.com/nmilford/rpm-activemq/master/activemq.init -O ~/rpmbuild/SOURCES/activemq.init`
 
`rpmbuild -bb ~/rpmbuild/SPECS/activemq.spec`
