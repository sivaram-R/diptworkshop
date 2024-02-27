# DIPTWORKSHOP
## AIM:
To Converte an image to gray scale and HSV.

## ALGORITHM:
1. Save any image and save the image with .jpg extension
2. Import cv module to work
3. Read the image using cv2.imread(‘image.jpg’) code
4. Similarly convert the image to grayscale and HSV and display the respectiveimage
5. To display the H,S and V plane, split the HSV image and showthe HUE, SATURATION and VALUE

## PROGRAM:
```python
import cv2
image=cv2.imread('flower.jpg',1)
image=cv2.resize(image,(400,300))
cv2.imshow('pic',image)
cv2.waitKey(0)
```
```python
import cv2
image = cv2.imread('flower.jpg')
image=cv2.resize(image,(400,300))
gray = cv2. cvtColor(image, cv2.COLOR_BGR2GRAY)
cv2. imshow('gray_scale', gray)
cv2. waitKey(0)
cv2. destroyAllWindows()
```
```python
import cv2
image = cv2.imread('flower.jpg')
image=cv2.resize(image,(400,300))
gray = cv2. cvtColor(image, cv2.COLOR_BGR2HSV)
cv2. imshow('my_img', gray)
cv2. waitKey(0)
cv2. destroyAllWindows()
```
```python
import cv2
image=cv2.imread("flower.jpg",1)
image=cv2.resize(image,(400,300))
image=cv2.cvtColor(image,cv2.COLOR_RGB2HSV)
H,S,V=cv2.split(image)
cv2.imshow('Hue',H)
cv2.imshow('Saturation',S)
cv2.imshow('Value',V)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
## OUTPUT:
![1](https://github.com/sivaram-R/diptworkshop/assets/121165794/1a131139-a60d-400a-a6af-bcc1e994ee7a)
![2](https://github.com/sivaram-R/diptworkshop/assets/121165794/d515794b-f015-4baa-a8bd-4e4f78eb66df)
![3](https://github.com/sivaram-R/diptworkshop/assets/121165794/111b5593-b0b2-4e23-bf00-1456cf325dd1)
![4](https://github.com/sivaram-R/diptworkshop/assets/121165794/b05f9d1e-bb86-4dbd-be9a-f9bd1771f480)

## RESULT:
Thus the image is converted to Grayscale and HSV.
