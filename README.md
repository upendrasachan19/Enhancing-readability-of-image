# Enhancing readability of Image

The readability of digital images of documents (especially Black and White) can be
greatly increased by removing the noise and enhancing image using adaptive threshold.

## Design details and implementation
### Assumptions
 - Generally, the content (text) is in black ink while the background (paper) is white coloured.
 - The document has exactly four straight edges (and hence the vertices)
 - The tilt of perspective from the top view is not more than 45 degrees.
 - Maximum portion of the image is covered by the document.
 - Nothing overlaps or obstructs the document in the image (like fingers, weights,
etc.).

### Steps
 - Detecting the edges of document [Canny Edge detection]
 - Using edges to find contour of the document 
 - Applying perspective transformation to obtain bird’s eye / top-down view of the
document.
- Enhancing image quality to increase readability [Adaptive thresholding]

## How to run

  - Install Python 27 and OpenCV
  - Copy the image in "images" folder
  - Run ```python final_script.py --image images/<image_name>.jpg```

You can view the original report from [here](https://www.slideshare.net/UpendraSachan4/enhancing-readability-of-digital-image-using-image-processing-full-report)
