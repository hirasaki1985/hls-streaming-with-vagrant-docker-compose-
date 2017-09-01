reverse_proxy template(with vagrant + docker-compose + jwilder/nginx-proxy)
====

vagrant + docker-compose + nginx-proxyで環境構築をする際のテンプレート

## Requirement
* Virtual Box
* vagrant
* /etc/hosts
* OBS

## Usage

## Install
```
$ git clone https://github.com/hirasaki1985/reverse_proxy.git
$ git checkout -b hls-streaming origin/hls-streaming
$ vagrant plugin install vagrant-vbguest
$ vagrant up
$ vi /etc/hosts
  192.168.33.10 web-server.com
  192.168.33.10 streaming-server.com
$ OBS setting
  * URL : rtmp://streaming-server.com:1935/hls
  * stream key : key
$ access your browser.
  http://web-server.com/
```

## 参考
```
https://github.com/brocaar/nginx-rtmp-dockerfile
```

## Licence

[MIT](https://github.com/hirasaki1985/reverse_proxy/raw/master/LICENSE)

## Author

[m.hirasaki](https://github.com/hirasaki1985)
