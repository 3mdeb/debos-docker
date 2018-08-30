Prerequisites
-------------

* `binfmt_misc` module loaded on the host machine:

```
modprobe binfmt_misc
```

Pull Docker image
-----------------

```
docker pull 3mdeb/debos-docker
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
debos-docker DEBOS_PARAMETERS
```

Build Docker image
------------------

> For development purposes only. Pull from dockerhub otherwise.

```
./build.sh
```

Release image to dockerhub
--------------------------

./release.sh VERSION_BUMP

`VERSION_BUMP` can be: `major`, `minor`, `patch`
