# docker-travis

https://docs.travis-ci.com/user/common-build-problems/#troubleshooting-locally-in-a-docker-image

### Ruby example

    docker run --name travis-debug -dit travisci/ci-garnet:packer-1512502276-986baf0 /sbin/init
    docker exec -it travis-debug bash -l
    su - travis
    git clone https://github.com/sinatra/sinatra.git
    cd sinatra
    bundle
