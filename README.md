# file_ios

This project patches the classical file type detecting command line tool `file` via [ios_system](https://github.com/holzschu/ios_system), for it to work in [iVim](https://github.com/terrychou/iVim) on iOS.

## Origin

The main source code of this project is `file-74.0.2.tar.gz`, obtained from Apple Open Source: https://opensource.apple.com/tarballs/file/

Please read its README for details.

## Some points if you want to build it

1. it depends on the framework `ios_system.framework` but it is not included in this repository. You may need to get it from the `ios_system` project;
2. you can find all the modifications in the code by searching for `FEAT_IOS`;
3. the `file` commmand needs magic definition files (as in the dir `Magdir`) to work properly, you need to make them availbale in your project by setting the environment variable `MAGIC`.

## Pull requests are welcome

If you find any problems or make any improvement based on this project, please do the pull request.
