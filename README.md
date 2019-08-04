# Multi Binary Executable Repo in Go

THe purpose of this repo is to show, how a Go repo can have more than one binary executable results. Just for the record. Here's the structure of the app:

~~~bash
.
├── cmd
│   ├── char
│   │   └── main.go
│   ├── defer
│   │   └── main.go
│   └── pointer
│       └── main.go
├── go.mod
└── README.md

4 directories, 5 files
~~~

Push them into the repo. To install into local bin repo:

```bash
$ go get -u -v github.com/oldstager/gomultibin/...
```

The results depend on the content of $GOPATH. They should reside in `$GOPATH/bin` (if you don't set
$GOPATH, they will be in `$HOME/go/bin` which is the default $GOPATH value.

