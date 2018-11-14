docker-gem5
===========

Dockerfile for automated gem5 build from public repositories on gem5.org

gem5 source directory is put in /usr/local/src/gem5
gem5 binary is in /usr/local/bin/gem5.opt

for more information visit http://gem5.org

```Bash
git clone https://github.com/ericvh/docker-gem5.git

cd docker-gem5

#build image
docker build -t gem5/ubuntu:v1 .

#docker run
docker run --name gem5 -it -v 'pwd'/workspace:/root/workspace gem5/ubuntu:v1 bash

#test gem5
/usr/local/bin/gem5.opt /usr/local/src/gem5/configs/example/se.py -c /usr/local/src/gem5/tests/test-progs/hello/bin/x86/linux/hello
```

