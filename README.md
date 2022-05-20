# Mathematical Edge Detection
This MATLAB project completed in my Advanved Engineering Mathematics course demonstrates gradient and Laplacian edge detection techniques, and their caveats with grayscale images.

## Important Takeaways
- Taking the gradient of an image in any direction (by convolving the image with a kernel) will result in an intuitive visualization of how quickly pixel values change in said direction. This can be used as a crude edge detection method.

![cameraman_horizontal_gradient](https://github.com/sebtona/mathematical-edge-detection/blob/main/images/image003.png) ![cameraman_vertical_gradient](https://github.com/sebtona/mathematical-edge-detection/blob/main/images/image004.png) ![cameraman_mag_gradient](https://github.com/sebtona/mathematical-edge-detection/blob/main/images/image005.png)

<img src="https://github.com/sebtona/mathematical-edge-detection/blob/main/images/image009.png" alt="peppers_horizontal_gradient" width="333" /> <img src="https://github.com/sebtona/mathematical-edge-detection/blob/main/images/image010.png" alt="peppers_vertical_gradient" width="333" /> <img src="https://github.com/sebtona/mathematical-edge-detection/blob/main/images/image011.png" alt="peppers_mag_gradient" width="333" />
- Taking the Laplacian of an image (again, by convolving the image with a kernel) will result in a visualzation of the rate at which the gradients change in any direction. This serves as a much cleaner and comprehensive edge detection method than trying to take gradients in individual directions.

![cameraman_laplacian](https://github.com/sebtona/mathematical-edge-detection/blob/main/images/image006.png) ![peppers_laplacian](https://github.com/sebtona/mathematical-edge-detection/blob/main/images/image012.png)
- The mapping of an RGB image to grayscale is a huge loss in information, and it opens your edge detection algorithm to vulnerabilities. Since many RGB color combinations will get mapped to the same grayscale value, an edge that could be detected in the original three-dimensional space may not be detected in the new one-dimensional space. This is demonstrated by example in my <a href="https://github.com/sebtona/mathematical-edge-detection/blob/main/project_report.pdf" target="_blank">project report</a>.

<img src="https://github.com/sebtona/mathematical-edge-detection/blob/main/images/image013.png" alt="example_rgb" width="500" /> <img src="https://github.com/sebtona/mathematical-edge-detection/blob/main/images/image014.png" alt="example_grayscale" width="485" />

<img src="https://github.com/sebtona/mathematical-edge-detection/blob/main/images/image015.png" alt="example_laplacian" width="325" /> <img src="https://github.com/sebtona/mathematical-edge-detection/blob/main/images/image016.png" alt="example_mag_gradient" width="325" />

## Run my Code
1. Download and install the latest version of MATLAB.
2. Fork this repo or download `mathematical_edge_detection.m`.
3. Open the `.m` file in MATLAB and click Run.
