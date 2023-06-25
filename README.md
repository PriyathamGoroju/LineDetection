# Line Detection from Image

This Python code is designed to detect and group lines from an image. It performs the following steps:

1. Loads an input image and converts it to grayscale.
2. Filters out pixels that are almost black and stores their coordinates.
3. Calculates the pairwise distances between all the filtered pixels.
4. Calculates the pairwise slopes (in degrees) between all the points.
5. Groups the points that have almost the same slope (within a specified threshold).
6. Groups the points that might belong to the same line based on their distances and slopes.
7. Plots the filtered pixels, slope-based groups, and line segments on a graph.

## Dependencies

- Python (version 3.6 or higher)
- OpenCV (cv2)
- NumPy
- Matplotlib

## Usage

1. Install the required dependencies using the following command:
```
pip install opencv-python numpy matplotlib
```
2. Place your input image file in the same directory as the code file.
3. Update the file name in the code to match your input image file.
4. Customize the threshold values for filtering pixels, grouping slopes, and line segment detection as per your requirements.
5. Run the code using the following command:
```
python line_detection.py
```

6. The program will display a graph showing the filtered pixels, slope-based groups, and line segments detected from the image.

## Customization

You can customize the following parameters in the code to adjust the line detection:

- `threshold`: The threshold value to filter out almost black pixels.
- `slope_threshold`: The threshold value for grouping points with similar slopes.
- `theta_threshold`: The threshold value for grouping points with similar thetas.
- `threshold_r`: The threshold value for grouping points with similar distances.

You can modify these parameters based on your specific use case to improve the line detection results.
