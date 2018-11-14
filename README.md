docker-gem5
===========

Dockerfile for automated gem5 build from public repositories on gem5.org

gem5 source directory is put in /usr/local/src/gem5
gem5 binary is in /usr/local/bin/gem5.opt

for more information visit http://gem5.org

cd docker-gem5
docker build -t gem5/ubuntu:v1 .
docker run --name gem5 -it -v 'pwd'/workspace:/root/workspace gem5/ubuntu:v1 bash
