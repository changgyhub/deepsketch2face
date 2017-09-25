# DeepSketch2Face

### Note: The database and the demo with bilinear encoding will be uploaded in the near future. Please keep staring if you need them.

Demo of [DeepSketch2Face: A Deep Learning Based Sketching System for 3D Face and Caricature Modeling](http://i.cs.hku.hk/~xghan/papers/deepske2face.pdf).
![Logo](http://i.cs.hku.hk/~xghan/Projects/ske2face_files/image004.gif)
We use Caffe modified from [Microsoft/Caffe](https://github.com/Microsoft/Caffe). Default Development OS is Windows 10 x64.

## Demo (Pure Alexnet Version)
0. Download repo [here](https://github.com/irsisyphus/deepsketch2face/archive/master.zip)
1. Download [caffemodel and dlls](https://www.dropbox.com/s/vub7drvu4tarybf/demo.zip?dl=0) and expand to `$(this_repo)\demo`
2. Install CUDA v8.0 (into `C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v8.0`). Other versions may not be supported.
3. Run `$(this_repo)\demo\deepsketch2face.exe`

## Demo (With bilinear encoding)
Comming in the near future

## Database
Comming in the near future

## Source Code Reproduction 
May not be uploaded.

0. Download source repo [here](TODO)
1. Install Visual Studio 2013 Ultimate
2. Install CUDA v8.0 (into `C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v8.0`) and cudnn v5.1 (copy files into `C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v8.0\cuda`). Other versions may not be supported.
3. Build `$(this_repo)\tools\caffe-master\windows\Caffe.sln` in Release x64. If there are errors, check if step 2 is correctly done.
4. Install Qt 5.8 (VS2013 x64). Other versions may not be supported.
5. If you use different Qt and Visual Studio version, you need to rebuild `$(this_repo)\tools\libQGLViewer\QGLViewer` in Qt Creator.
6. In `$(this_repo)\tools\caffe-master\include\caffe\proto\caffe.pb.h`, change "STRICT" in line 2525 and 9794 into "_STRICT"
7. Open `$(this_repo)\src\deepsketch2face.pro` in Qt Creator, set build directory to `$(this_repo)\build`, then build the program in Release.
8. Copy `$(this_repo)\build\release\deepsketch2face.exe` into `$(this_repo)\demo`
9. For all `.dll` file in `$(this_repo)\demo` and `$(this_repo)\demo\platforms`, if you build the program in different settings, you may need to change them correspondingly. A safe but redundant move is to copy all `.dll` file in `$(this_repo)\tools\` and Qt here.
10. Run `$(this_repo)\demo\deepsketch2face.exe`
