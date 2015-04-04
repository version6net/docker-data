# docker-data

**Description**

Dockerfile for Data Volume Container

**Building**

```
docker build -t v6net/data .
```

**Usage**

First run data volume container you just created

```
docker run --name datavolume v6net/data
```

Then run your application container which uses /data volume

```
docker run --volumes-from datavolume ....
```

**Cleanup**

```
docker rm datavolume
```
