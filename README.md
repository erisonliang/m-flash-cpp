# M-Flash: Fast billion-scale graph computation using a bimodal block processing model

## Dependencies
* [EasyLogging++](http://easylogging.muflihun.com). It is included in M-Flash
* [Boost](http://www.boost.org) (CentOS yum install boost boost-devel)
* [Eigen3](http://eigen.tuxfamily.org/). It is required for Lanczos Selective Orthogonalization

## Examples

### Pagerank 
```
cd [M-FLASH_ROOT];
make example_apps/pagerank
bin/example_apps/pagerank file [FILE_GRAPH] niters 4
```

### Weakly Connected Components (Iterative)
```
cd [M-FLASH_ROOT];
make example_apps/wcc
bin/example_apps/wcc file [FILE_GRAPH] iterative 1 niters 4 
```
Iterative until convergency
```
cd [M-FLASH_ROOT];
make example_apps/wcc
bin/example_apps/wcc file [FILE_GRAPH] iterative 1 
```

### Weakly Connected Components (Union-Find)
```
cd [M-FLASH_ROOT];
make example_apps/wcc
bin/example_apps/wcc file [FILE_GRAPH] iterative 0 
```


## License
M-Flash is licensed under the Mozilla Public License, Version 2.0. 
