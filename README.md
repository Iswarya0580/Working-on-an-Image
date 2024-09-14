# Working-on-an-Image
## Name : Iswarya P
## Register No : 212223230082

## Program:

```
import cv2
image1=cv2.imread('img1.jpg')
image2=cv2.imread('img2.jpg')

image1.shape
image2.shape

image1_resized=cv2.resize(image1,(400,400))
image2_resized=cv2.resize(image2,(400,400))

image1_resized.shape
image2_resized.shape

R1 = image1_resized[0:200, 0:200]      # Top-left region
R2 = image1_resized[0:200, 200:400]  # Top-right region
R3 = image1_resized[200:400,0:200] # Bottom-left region
R4 = image1_resized[200:400,200:400] # Bottom-right region

R5 = image2_resized[0:200, 0:200]      # Top-left region
R6 = image2_resized[0:200, 200:400]  # Top-right region
R7 = image2_resized[200:400,0:200] # Bottom-left region
R8 = image2_resized[200:400,200:400] # Bottom-right region

image1_resized[0:200,0:200]=R8
image2_resized[200:400,200:400]=R3

cv2.imshow('Resized Image 1',image1_resized)
cv2.imshow('Resized Image 2',image2_resized)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

## Output:

![Screenshot 2024-09-14 110649](https://github.com/user-attachments/assets/76379a92-a80f-4ad5-bfb7-3ea93c675f43)


![Screenshot 2024-09-14 110655](https://github.com/user-attachments/assets/feb8daa0-46f2-4a94-9d87-125d56eca9ca)

![Screenshot 2024-09-14 102829](https://github.com/user-attachments/assets/29de4a5a-043d-4d81-8c6c-f6c8b9ef8baa)

## Result:
Thus the code to working on an image was executed successfully.
