## Build My World

A 4 wheeled small robot housed in a one floor flat.


### Building the plugin

With `$PROJECT_ROOT` containing the clone destination directory

Build the plugin:

```shell
$ cd $PROJECT_ROOT
$ mkdir -p build
$ cd build/
$ cmake ../
$ make
```
Path the library/plugin

``` shell
$ cd $PROJECT_ROOT && export GAZEBO_PLUGIN_PATH=${GAZEBO_PLUGIN_PATH}:$(pwd)/build
```

## Launch gazebo (after exporting the plugin path)
```shell
$ gazebo world/housed_4_wheeled.world
```

![housed4wheeled](images/housed_4_wheeled.png)

