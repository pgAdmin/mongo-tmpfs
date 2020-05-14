# mongo-tmpfs
[mongo-tmpfs](https://hub.docker.com/r/pgadmin/mongo-tmpfs) is a docker container for running a mongo instance against a tmpfs storage volume.

This container is designed to enhance performance in testing environments. Logging and preallocation is disabled and smallfiles are enabled.

The `TMPFS_SIZE` environment variable can be used to configure the size (in MB) of the tmpfs volume.

```
docker run  --name mongo-tmpfs \
            --privileged \
            -p 27017:27017 \
            pgadmin/mongo-tmpfs:4.0
```

## MongoDB Version
Different version of the mongo-tmpfs container are available for different versions.

| Mongo Version  | Docker Tag                   |
| -------------- | ---------------------------- |
| 3.6            | pgadmin/mongo-tmpfs:3.6 |
| 4.0            | pgadmin/mongo-tmpfs:4.0 |
