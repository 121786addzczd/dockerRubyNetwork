# introduction-to-docker

## 起動手順

```
cd sinatra
docker build -t my-ruby:dockerfile .
cd ..
docker run \
  -v $PWD/sinatra:/opt/myapp \
  -w /opt/myapp \
  my-ruby:dockerfile \
  ruby myapp.rb
```
