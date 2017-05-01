# Headless Chrome Docker Image

## Pull or Build

### pull
```
$ docker pull lenaten/headless-chrome
```

### build
```
$ docker build -t lenaten/headless-chrome .
```

## Run
```
$ docker run -d -p 9222:9222 --privileged lenaten/headless-chrome --headless --disable-gpu --remote-debugging-port=9222 --remote-debugging-address=0.0.0.0 https://www.google.com
```

## Connect
```
$ open http://localhost:9222
```