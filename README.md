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

Homogeneous Blur is the most simplest method of smoothing an image. It is also called as Homogeneous Smoothing, Homogeneous Filtering and Box Blurring. In this technique, each pixel value is calculated as the average value of the neighborhood of the pixel defined by the kernel.

Kernels used in the homogeneous blur is called normalized box filter. You may define any size for this kernel according to  your requirement. But it is preferable to define square kernels with a size of odd width and height.

Gaussian blur/smoothing is the most commonly used smoothing technique to eliminate noises in images and videos. In this technique, an image should be convolved with a Gaussian kernel to produce the smoothed image.
You may define the size of the kernel according to your requirement. But the standard deviation of the Gaussian distribution in X and Y direction should be chosen carefully considering the size of the kernel such that the edges of the kernel is close to zero. Here I have shown the 3 x 3 and 5 x 5 Gaussian kernels.
OpenCV has an in-built function to perform Gaussian blur/smoothing on images easily. All you have to specify is the size of the Gaussian kernel with which your image should be convolved.

Erosion is a fundamental morphological operation in image processing. As the name implies, this operation erodes foreground pixels in an image at their boundaries. After this erosion operation is performed, objects in an image becomes smaller where as the holes within the object (if any) becomes larger.

In this technique, each pixel value of the resultant image is calculated as the minimum value of the neighborhood of the pixel defined by the kernel. For color images, each color plane is processed independently.

Most of the Information and Code is taken from OpenCV Tutorial C++
