Mozilla RelEng Linux Build Environments
=======================================

Mock configs and Dockerfiles for generating build environments, with packages installed from Mozilla's RelEng repositories.

##Images published to docker.io:

###Builders: with dependencies from <a href="https://github.com/mozilla/build-mozharness">Mozharness</a> configs

####Linux 64 (Releng Base Builder)
https://registry.hub.docker.com/u/mrrrgn/releng_base_linux_64/

####Linux 32 (Releng Base Builder)
https://registry.hub.docker.com/u/mrrrgn/releng_base_linux_32/

###Platform: no build specific libraries

####Linux 64
https://registry.hub.docker.com/u/mrrrgn/mozilla-centos6-x86_64/

####Linux 64 + Android (Mozilla Java Packages)
https://registry.hub.docker.com/u/mrrrgn/mozilla-centos6-x86_64-android/

####Linux 32
Note: The environment is 64 bit; but you can "trick" programs into seeing a 32 bit system by prefixing all commands with `linux32`. This image is pointed at Mozilla's 32 bit mirror, so be sure to use that prefix before installing packages.

https://registry.hub.docker.com/u/mrrrgn/mozilla-centos-i386/

## About
These containers may be useful for Firefox Developers trying to debug issues which appear on our in house CI servers. For instance, you can be sure that you're using the same libraries and compilers:
<img src="yum.png"></img>
<img src="env.png"></img>
