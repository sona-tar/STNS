# Simple Toml Name Service
[![Build Status](https://travis-ci.org/STNS/STNS.svg?branch=master)](https://travis-ci.org/STNS/STNS)

STNS is used by sshd to access keys and user resolver provided

You can see the details of STNS on [stns.jp](http://stns.jp)

```
$ ssh pyama@example.jp
$ id pyama
uid=1001(pyama) gid=1001(pyama) groups=1001(pyama)
```

![overview](https://cloud.githubusercontent.com/assets/8022082/13373974/250a8b16-ddba-11e5-994d-b1bbc81a6b94.png)

## Let's Trial
can you trial STNS by docker.

```
$ git clone https://github.com/STNS/STNS.git
$ cd example
$ docker build -t stns:trial .
$ docker run -t stns:trial
[root@67f8941ad374 /]# id example
uid=1001(example) gid=1001(example) groups=1001(example)
```

## blog
* [Linuxユーザーと公開鍵を統合管理するサーバ&クライアントを書いた](https://ten-snapon.com/archives/1228)
* [デプロイユーザーをSTNSで管理する](https://ten-snapon.com/archives/1330)
* [STNSに組織体系を管理するLinkGroup機能を追加しi386に対応しました](https://ten-snapon.com/archives/1346)
* [STNSでSudoパスワードをサポートした](https://ten-snapon.com/archives/1355)
* [パスワード暗号化について学びを得た](https://ten-snapon.com/archives/1399)

# VS
## LDAP
LDAP is used convenient and very well
However, sometimes it becomes complicated and versatile too.
STNS function is small compared with the LDAP, but it is management that much simple.
And, In many cases, meet the required functionality.

## author
* pyama86
