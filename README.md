# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:

Import the necessary packages.

### Step2:

Create the text image using cv2.putText.

### Step3:

Then create the structuring image for dilation/erosion.

### Step4:

Apply erosion and dilation using cv2.erode and cv2.dilate.

### Step5:

Plot the images using plt.imshow.

 
## Program:

``` 
import cv2
import numpy
NameImage = numpy.zeros((100,1000),dtype='uint8')
font = cv2.FONT_ITALIC
cv2.putText(NameImage,'D.R.Vinuthna',(50,70),font,2,(255),5,cv2.LINE_4)
cv2.imshow("Name Image",NameImage)
kernel1 = cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
erodeImage = cv2.erode(NameImage,kernel1)
dilationImage = cv2.dilate(NameImage,kernel1)
cv2.imshow("Erode Image",erodeImage)
cv2.imshow("Dilated Image",dilationImage)
cv2.waitKey(0)

cv2.destroyAllWindows()


```
## Output:

### Display the input Image

![output](https://github.com/VINUTHNA-2004/Implementation-of-Erosion-and-Dilation/blob/main/ex10-a.png?raw=true)


### Display the Eroded Image

![output](https://github.com/VINUTHNA-2004/Implementation-of-Erosion-and-Dilation/blob/main/ex10-b.png?raw=true)


### Display the Dilated Image

![output](https://github.com/VINUTHNA-2004/Implementation-of-Erosion-and-Dilation/blob/main/ex10-b.png?raw=true)

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
