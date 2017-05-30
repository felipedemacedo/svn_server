# Ubuntu Server 16.04 with Subversion installed.

## Usage example:
```console
docker run -ti -v /c/HOST_SVN_DIRECTORY:/CONTAINER_SVN_DIRECTORY --name svn_container -p HOST_PORT:2402 -d felipederodrigues/svn
```

docker exec -ti svn_container /bin/sh -c "cd /CONTAINER_SVN_DIRECTORY && svnserve --listen-port 2402 -d"

@TEST IT !
svn://HOST_IP_ADDRESS:HOST_PORT/CONTAINER_SVN_DIRECTORY