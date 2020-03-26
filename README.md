# Filters-and-Histogra-in-Open-CV
A histogram is a statistical graphic representation of variable distribution. This
allows us to understand the density estimation and probability distribution of data.
If we apply this histogram concept to an image, it seems to be complex to
understand, but it is really very simple. In a gray image, our variable values can
take any possible gray value ranging from 0 to 255, and the density is the number
of pixels in the image that have this value. This has been done in Drawing a Histogram.

Histogram equalization is a commonly used technique in image processing to enhance the contrast of an image by equalizing the intensity distribution.
It will make a dark image (underexposed) less dark and a bright image (overexposed) less bright. 
But practically, it is hard to achieve this kind of perfect histogram equalization. However there are various techniques to achieve histogram equalization close to the perfect one. 
In OpenCV, there is an in-built function to equalize the histogram.(In Histogram of a grayscale image, colour image and Video
Most of the Information and Code is taken from OpenCV Tutorial C++
