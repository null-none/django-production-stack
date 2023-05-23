# django-production-stack

### Prerequisites
- Docker
- Familiarity with Docker Compose.

### Development
Just build your django app on top of ```/volumes/app```

### Deployment commands
```bash
docker-compose up
docker-compose down
```

### Notes

- About python docker base image:

    <blockquote>I’d probably choose the official Docker Python image (python:3.11-slim-bullseye).</blockquote>
    
    See this [link](https://pythonspeed.com/articles/base-image-python-docker-images/).

- To deploy Distributed MinIO on Docker Compose:
    https://github.com/minio/minio/tree/master/docs/orchestration/docker-compose

- To change Nginx-Modsecurity configuration:
    Replace ```/volumes/nginx/default.conf```

- Leave ```REDIS_USER``` blank if you use redis default user.
