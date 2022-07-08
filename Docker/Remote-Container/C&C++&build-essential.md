## 注意
- apt-get updateを削除しているので、新しくinstallするときは、また`apt update`する必要がある
```dockerfile
FROM ubuntu:latest

RUN apt-get update && \
    apt-get install -y --no-install-recommends && \
    gcc && \
    g++ && \
    build-essential && \
    rm -rf /var/lib/apt/lists/*

WORKDIR /tm
```
