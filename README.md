# docker image for ruby-1.8.7 with rails-2.3.18 on ubuntu xenial

see detail: https://github.com/bellbind/docker-ruby18-rails2/blob/master/Dockerfile

Include gems:

- sqlite3
- mecab
- mongrel
- rake

You can run a rails-2.3 app as:

```
docker run -it --rm -v $(pwd)/my-rails-app:/root/app -w /root/app -p 3000:3000  bellbind/docker-ruby18-rails2 ruby script/server
```
