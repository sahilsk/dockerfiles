Build Image


    docker pull sahilsk/ruby

Run containers

    root@pblin050:/opt/dockerize/base# docker run -it --rm sahilsk/ruby /bin/bash
    [ root@9f7acba75316:~ ]$ ruby -v
    ruby 2.1.2p95 (2014-05-08 revision 45877) [x86_64-linux]
    [ root@9f7acba75316:~ ]$ rbenv -v
    rbenv 0.4.0-98-g13a474c
    [ root@9f7acba75316:~ ]$


To update ruby version

        root@pblin050:/opt/dockerize/base# docker run -it sahilsk/ruby /bin/bash
        [ root@9f7acba75316:~ ]$ ruby -v
        ruby 2.1.2p95 (2014-05-08 revision 45877) [x86_64-linux]
        [ root@9f7acba75316:~ ]$ rbenv install -l
    ...
     2.1.2
     2.1.3
     2.1.3
    ...
    [ root@9f7acba75316:~ ]$ rbenv install 2.1.3
    Downloading ruby-2.1.3.tar.gz...
    -> http://dqw8nmjcqpjn7.cloudfront.net/0818beb7b10ce9a058cd21d85cfe1dcd233e98b7342d32e9a5d4bebe98347f01 ...
     [ root@9f7acba75316:~ ]$ rbenv local 2.1.3
     [ root@9f7acba75316:~ ]$ rbenv global 2.1.3
     [ root@9f7acba75316:~ ]$ ruby -v

