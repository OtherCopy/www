Installation
---------------

```sh
go get github.com/pocke/www
```

You download binary from [latest release](https://github.com/pocke/www/releases/latest), and place it in `$PATH` directory.

Usage
---------

```sh
cd DOCUMENT_ROOT
www
```

HTTP Server start serving for static files at random port. And browser is automatically opened.

```sh
Usage of www:
  -b, --binding="localhost": Bind www to the specified IP.
  -p, --port=0: TCP port number
```

![www-basic](http://cdn-ak.f.st-hatena.com/images/fotolife/P/Pocke/20160125/20160125120042.gif)


Configuration file
------

www loads `./.www` file as command line options.

```sh
$ cat .www
-p 8888
$ www
http://127.0.0.1:8888
2016/07/22 17:04:28 Started GET "/" for 127.0.0.1:49500
2016/07/22 17:04:28 response status: 200
...
```


VS. python3 -m http.server
-------------------------

|              | python         | www |
| ---          | -----          | --- |
| port         | 8000(Optional) | Random |
| browser open | Manual         | automatically |
| command name | long           | short |


Re-open the browser
---------


![www-reload](http://cdn-ak.f.st-hatena.com/images/fotolife/P/Pocke/20160125/20160125120207.gif)

Links
-------

- [楽々静的HTTPサーバー - pockestrap](http://pocke.hatenablog.com/entry/2016/01/25/120952)
- [www v0.3.0 をリリースした - pockestrap](http://pocke.hatenablog.com/entry/2016/04/09/233321)


License
-------

These codes are licensed under CC0.

[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png "CC0")](http://creativecommons.org/publicdomain/zero/1.0/deed.en)
