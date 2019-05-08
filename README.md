# dockerfiles

Various Dockerfiles for simple images I use in various places.
Inspired by https://github.com/jessfraz/dockerfiles .

## Images

Most of these should be findable on dockerhub under cerebrate/whatever.

## The Containers

| Container                     | Purpose                                                         |
|-------------------------------|-----------------------------------------------------------------|
| czsh                          | minimal zsh/oh-my-zsh on debian, for testing                    |
| emacs                         | containerized emacs, no X.                                      |
| htop                          | process monitoring                                              |
| httpbin                       | simple HTTP request/response service ( https://httpbin.org/ )   |
| httpie                        | intuitive CLI HTTP client ( https://httpie.org/ )               |
| netcat                        | the tcp swiss army knife                                        |
| python:3-with-buildessentials | python:3-slim-sid with build-essential installed (intermediate) |

Containers noted as (intermediate) are used only as build steps for other containers.
