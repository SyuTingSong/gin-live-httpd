# gin live httpd

Live edit and compile go source code and restart web server based on [codegangsta/gin](https://github.com/codegangsta/gin).

The [gin-gonic/gin](https://github.com/gin-gonic/gin) web framework is included.

## Usage

```sh
cd path/to/your/gin/project
docker run -ti --rm \
    -v $(pwd):/app \
    -p 8080:80 \
    syutingsong/gin-live-httpd
```

## Environment Variables

Name | Desc | Default
---|---|---
GIN_LADDR | listening address for the proxy server | 0.0.0.0
GIN_PORT | port for the proxy server | 80
BIN_APP_PORT | port for the Go web server | 3001
GIN_BIN | name of generated binary file | gin-bin
GIN_BUILD_ARGS | Additional go build arguments |
GIN_CERT_FILE | TLS Certificate |
GIN_KEY_FILE | TLS Certificate Key |
GIN_LOG_PREFIX | Log prefix | gin

