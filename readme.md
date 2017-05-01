# Headless Chrome Docker Image

```
$ docker pull lenaten/headless-chrome
```

## Build
```
$ docker build -t chrome .
```

## Run
```
$ docker run -d -p 9222:9222 --privileged chrome  --headless --disable-gpu --remote-debugging-port=9222 --remote-debugging-address=0.0.0.0 https://www.google.com
```

## Connect
```
$ open http://localhost:9222
```