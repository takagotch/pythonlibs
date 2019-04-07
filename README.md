### pythonlibs
---
https://www.lfd.uci.edu/~gohlke/pythonlibs/

numpy-opencv-converter
https://github.com/spillai/numpy-opencv-converter

```cc
cv::Mat process_mat(const cv::Mat& in) {
  cv::Mat out = in.clone();
  return out;
}

boost::python::deg("process_mat", &process_mat);

import numpy as np
from cv_module import process_mat
A = np.random.random(shape=(4,3))
B = process_mat(A)
```

```
git clone git@github.com:spillai/numpy-opencv-converter
mkdir build
cd build && cmake ..
make
```

```
```


