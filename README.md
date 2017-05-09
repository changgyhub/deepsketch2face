# DeepSketch2Face
Demo of [DeepSketch2Face: A Deep Learning Based Sketching System for 3D Face and Caricature Modeling](http://i.cs.hku.hk/~xghan/papers/deepske2face.pdf).
![Logo](http://i.cs.hku.hk/~xghan/Projects/ske2face_files/image004.gif)
## Demo (beta version) - COMMING SOON
### Known Bugs:
1. Texture may not be correctly displayed. We will fix this bug soon.
2. Sometimes the program fails to load current folder name. The bug results from QDir::currentPath() which has synchronization issues. Since Caffe Networks need to be pre-defined globally, a hard-code solution might be unreasonable. We will fix this bug soon. We encourage you to restart the program if such bug occurs.
3. Moving the program window may cause shift in transparent drawing window. We advice you not to move the program window.

### Setup - ON CONSTRUCTION
1. Building our version of caffe [here](https://github.com/irsisyphus/deepsketch2face), modified from [Microsoft/caffe](https://github.com/Microsoft/caffe).
2. Download our models from [here](https://github.com/irsisyphus/deepsketch2face). Expand it into demo folder.
3. run `Paint.exe`

## Database - COMMING SOON
