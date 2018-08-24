Building
--------

```
./build.sh
```

Prerequisites
-------------

* `binfmt_misc` module loaded on the host machine:

```
modprobe binfmt_misc
```

Running
-------

```
./run.sh DEBOS_PARAMETERS
```

> Visit [debos repo](https://github.com/go-debos/debos) for tool usage

For easy access from any directory:

```
ln -s $(readlink -f run.sh) ~/bin/debos-docker
```
