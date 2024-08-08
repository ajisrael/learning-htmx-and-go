# Learning HTMX & Go

## Introduction

### Links
    - [Course](https://theprimeagen.github.io/fem-htmx/)
    - [HTMX Docs](https://htmx.org/docs/)
    - [HTMX Book](https://hypermedia.systems/)

### Setup

[Install Golang](https://go.dev/doc/install)

Install Air

```bash
go install github.com/air-verse/air@latest
```

Install LSP

```bash
go install golang.org/x/tools/gopls@latest
```

* Note: may need to enable in nvim

Project Setup

```bash
git clone git@github.com:ThePrimeagen/fem-htmx-proj.git
cd fem-html-proj
go mod init mywebsite.tv/name
```

### HATEOAS

Hypermedia As The Engine Of Application State

### General Flow

```bash
╭─----------------─---╮ ----- VERB /path ----> ╭─--─----╮
| <el hx-VERB="path"> |                        | Server |
╰─----------------─---╯ <------ <html> ------- ╰─-------╯

* contents of <html> will replace the innerHTML of *
    el if the request responded with 200
```


