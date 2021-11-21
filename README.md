# Bicubic-interpolation
This repository is for simple implementation of 'Bicubic-interpolation for images' (Python3).

## Table of contents
  * [Formulation](#Formulation)
  * [Example](#Example)
  * [Requirement](#Requirement)
  * [Installation](#Installation)
  * [Usage](#Usage)
  * [Reference](#Reference)
  * [Credits](#Credits)

## Formulation
  * Interpolation kernel [1]

  &emsp;&emsp;![Formulation](/img/formulation.png)

  * Interpolation
  Use the values of 16 pixels around the new pixel dst(x,y) [1][2]. (x,y) shows the location of pixels.

  &emsp;&emsp;![Formulation2](/img/formulation2.png)

  Here, f means the values of pixels. x1, x2, x3, x4 are the distance of x direction from new pixel to near 16 pixels. y1, ... are the distance of y direction.

## Example
  * Upscale input image 2 times (ratio = 2)
  The 'butterfly' image is from [3].

  &emsp;&emsp;![Input image](/img/butterfly.png)

  &emsp;&emsp;↑ Input image (256x256)

  &emsp;&emsp;![Output image](/img/bicubic_butterfly.png)

  &emsp;&emsp;↑ Output image (512x512)

## Requirement
  * Python 3.5.2 or more - `$ python --version` or `$ python3 --version`
  * numpy and opencv modules `$ pip3 freeze -r requirements.txt`

## Installation
`$ git clone https://github.com/Kel-1-Cabang-GitHub/bicubic-interpolation.git`

## Usage
  1. `$ python src\bicubic.py`
  2. `$ python3 src\bicubic.py`

## Reference
  1. R. Keys, "Cubic convolution interpolation for digital image processing," in IEEE Transactions on Acoustics, Speech, and Signal Processing, vol. 29, no. 6, pp. 1153-1160, December 1981. URL: <http://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=1163711&isnumber=26156>
  2. 奥富正敏ら, "ディジタル画像処理[改定新版]", CG-ARTS協会, pp. 170-171, 2016.
  3. M. Bevilacqua, A. Roumy, C. Guillemot and ML. Alberi, "Low-Complexity Single-Image Super-Resolution based on Nonnegative Neighbor Embedding",BMVC 2012.
  4. https://github.com/yunabe/codelab/blob/master/misc/terminal_progressbar/progress.py to show the progress.

## Credits
  [@rootpine](https://github.com/rootpine/)