---
title: "OpenCV3 installation with Python 3 using conda"
date: 2017-08-14 08:26:28
categories: 01_Install 
tags: OpenCV_Python OpenCV conda
---

# OpenCV3 설치 (Conda, Python3)
@(Python)[01_install conda]

### conda의 opencv를 위한 환경 생성

```
conda create -n opencv python=3
```

### 생성한 opencv를 위한 환경 확인

```
conda env list
```

opencv가 나오면 문제없이 생성된 것임.

### 생성한 opencv 환경 활성화

```
conda activate opencv
```

### opencv3 관련 정보 확인.

```
anaconda show menpo/opencv3
```

### opencv3 설치

```
conda install --channel https://conda.anaconda.org/menpo opencv3
```

### jupyter lab설치

```
conda install jupyterlab
```

### Error 발생 

2019.6.19 현재 `import cv2`를 하면 에러가 뜨고 동작을 안함. 
이를 해결하기 위해 googling을 했고 다음으로 해결함.

```
conda install -c asmeurer pango
```

for detail, refer (https://github.com/ContinuumIO/anaconda-issues/issues/368)
