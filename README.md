reverse_proxy template(with vagrant + docker-compose + jwilder/nginx-proxy)
====

vagrant + docker-compose + nginx-proxyで環境構築をする際のテンプレート

## Requirement
* Virtual Box
* vagrant
* /etc/hosts

## Usage

## Install
```
$ git clone https://github.com/hirasaki1985/reverse_proxy.git
$ cd reverse_proxy
$ vagrant plugin install vagrant-vbguest
$ vagrant up
$ vi /etc/hosts
  192.168.30.10 web-project01
  192.168.30.10 web-project02
$ access your browser.
  http://web-project01.com
  http://web-project02.com
```

## Licence

[MIT](https://github.com/hirasaki1985/reverse_proxy/raw/master/LICENSE)

## Author

[m.hirasaki](https://github.com/hirasaki1985)
