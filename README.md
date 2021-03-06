# BeautyR

<img src="img/logo.png" align="right" height="200" width="200"/>

Image processing in R.

## Contributors

[Gilbert Lei](https://github.com/gilbertlei)

[Jielin Yu](https://github.com/jielinyu)

[Olivia Lin](https://github.com/olivia-lin)

## Overview
Nearly everyone has some experience with Image processing, which is around our daily life. For example, when we use iPhone's camera to take pictures, it allows us to choose a filter which can add some special effects on these pictures. While using these filters, people might have wondered how these special effects are realized.

We developed this package that performs digital image processing on .jpg images. People can use it to transform images into new images with some special effects, such as embossing, to compress images to reduce file sizes, and to calculate the exact number of bytes an image has. We hope to advance and add more functions later on.  

## Functions
**Emboss**  
This function turns a colorful image into an embossment-style image. It replaces each pixel of the image by either a highlight or a shadow. Low contrast areas are replaced by a gray background.

**Compress**  
This function compresses an image by 50% on both height and width dimensions. It uses seam-carving method to remove low energy pixels and reduce the size of the original image. Output image may look a little bit different from the original image.  

**Calculate_Bytes**  
This function calculates the bytes size of an image.

## Similar Packages in R

There are packages in R to compress images
[magick package](https://cran.r-project.org/web/packages/magick/vignettes/intro.html)

Function `object.size` works as the same as our function `Calculate_Bytes` [object.size](https://stat.ethz.ch/R-manual/R-devel/library/utils/html/object.size.html)

Function `edge.detect` works as the same as our function `sketch`, which can detect image's edge.
It is achieved by using method "canny". [edge.detect](https://www.rdocumentation.org/packages/wvtool/versions/1.0/topics/edge.detect)
