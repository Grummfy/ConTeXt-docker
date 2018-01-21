# ConTeXt-docker
A docker to run ConTeXt command and output files.

[Context home](http://wiki.contextgarden.net/)

More information on commands you can run: http://www.pragma-ade.com/general/manuals/tools-mkiv

Compile your ConTeXt document:

```
docker run -ti --rm -v ${PWD}:/my-doc -w /my-doc grummfy/ConTeXt-docker context your-doc.tex
```

if `your-doc.tex` is inside the current directory (the current directory is mounted in the docker through ${PWD)}


## Why this docker?

With this docker, you imagine to use it to build inside a continuous building plateform, your documents and make it available automatically.
This is my usage ;)
