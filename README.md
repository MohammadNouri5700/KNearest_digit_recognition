# KNearest_digit_recognition

I took below image for my training data:

[![Sample Numbers](https://raw.githubusercontent.com/MohammadNouri5700/KNearest_digit_recognition/main/data/samplenumbers.png "Sample Numbers")](https://raw.githubusercontent.com/MohammadNouri5700/KNearest_digit_recognition/main/data/samplenumbers.png "Sample Numbers")

( I know the amount of training data is less. But, since all letters are of same font and size, I decided to try on this).

------------

To prepare the data for training, I made a small code in OpenCV. It does following things:

1. It loads the image.
2. Selects the digits ( obviously by contour finding and applying constraints on area and height of letters to avoid false detections).
3. Draws the bounding rectangle around one letter and wait for key press manually. This time we press the digit key ourselves corresponding to the letter in box.
4. Once corresponding digit key is pressed, it resizes this box to 10x10 and saves 100 pixel values in an array (here, samples) and corresponding manually entered digit in another array(here, responses).
5. Then save both the arrays in separate txt files.

At the end of manual classification of digits, all the digits in the train data( train.png) are labeled manually by ourselves, image will look like below:

[![samplenumbers_result](https://raw.githubusercontent.com/MohammadNouri5700/KNearest_digit_recognition/main/data/samplenumbers_result.png "samplenumbers_result")](http://https://raw.githubusercontent.com/MohammadNouri5700/KNearest_digit_recognition/main/data/samplenumbers_result.png "samplenumbers_result")


Here it worked with 100% accuracy. I assume this is because all the digits are of same kind and same size.

[![result](https://raw.githubusercontent.com/MohammadNouri5700/KNearest_digit_recognition/main/result.PNG "result")](https://raw.githubusercontent.com/MohammadNouri5700/KNearest_digit_recognition/main/result.PNG "result")


