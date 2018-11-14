### Usage example:

```Shell
$ cd lab # student lab directory
$ git submodule update --init
$ docker run  -v `pwd`:`pwd` -w `pwd` -i -t rusdevops/devenv-cpp
$ scripts/tests.sh
$ mkdir _coverage && find . -name "*.gcov" -exec mv -t _coverage {} \+
$ vim -c "GcovFind" sources/source.cpp
```
