# Mathematical Edge Detection
This MATLAB project completed in my Advanved Engineering Mathematics course demonstrates gradient and Laplacian edge detection techniques, and their caveats with grayscale images.

## Important Takeaways
- Taking the gradient of an image in any direction (by convolving the image with a kernel) will result in an intuitive visualization of how quickly pixel values change in said direction. This can be used as a crude edge detection method.
- Taking the Laplacian of an image (again, by convolving the image with a kernel) will result in a visualzation of the rate at which the gradients change in any direction. This serves as a much cleaner and comprehensive edge detection method than trying to take gradients in individual directions.
- The mapping of an RGB image to grayscale is a huge loss in information, and it opens your edge detection algorithm to vulnerabilities. Since many RGB color combinations will get mapped to the same grayscale value, an edge that could be detected in the original three-dimensional space may not be detected in the new one-dimensional space. This is demonstrated by example in my <a href="https://github.com/sebtona/mathematical-edge-detection/blob/main/project_report.pdf" target="_blank">project report</a>.

## Run my Code
1. Download and install the latest version of MATLAB.
2. Fork this repo or download `mathematical_edge_detection.m`.
3. Open the `.m` file in MATLAB and click Run.
