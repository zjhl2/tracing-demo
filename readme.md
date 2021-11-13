# tracing-demo (using jaeger)

- https://www.jaegertracing.io/
- https://github.com/yurishkuro/opentracing-tutorial/

## 1. run jaeger-all-in-one
``` dockerfile
docker run -d --name jaeger \
  -e COLLECTOR_ZIPKIN_HOST_PORT=:9411 \
  -p 5775:5775/udp \
  -p 6831:6831/udp \
  -p 6832:6832/udp \
  -p 5778:5778 \
  -p 16686:16686 \
  -p 14268:14268 \
  -p 14250:14250 \
  -p 9411:9411 \
  jaegertracing/all-in-one:1.28
```

## 2. run formatter and publisher, then hello

## 3. open https://localhost:16686