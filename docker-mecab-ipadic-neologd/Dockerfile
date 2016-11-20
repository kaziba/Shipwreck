FROM ubuntu:latest

RUN apt-get update
RUN apt-get upgrade -y

# Build essentials
RUN apt-get install -y libc6-dev curl build-essential mecab libmecab-dev mecab-ipadic-utf8 git make xz-utils file

# Mecab
RUN ["mecab", "-h"]

# Clean up
# RUN apt-get remove -y build-essential
# RUN rm -rf mecab-0.996.tar.gz*
# RUN rm -rf mecab-ipadic-2.7.0-20070801*

# mecab-ipadic-neologd
RUN git clone https://github.com/neologd/mecab-ipadic-neologd.git
RUN cd mecab-ipadic-neologd && ( echo yes | ./bin/install-mecab-ipadic-neologd )
# Dockerfile で cd が効かない - Carpe Diem http://christina04.hatenablog.com/entry/2014/10/31/101510

ENTRYPOINT mecab -d /usr/local/lib/mecab/dic/mecab-ipadic-neologd/