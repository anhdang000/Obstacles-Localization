# Estimating Obstacle Positions in KITTI Dataset using U and V-Disparity with Simple Geometric Implementation

##  Processing pipeline:
1. Read image
2. Convert to grayscale
3. Compute obstacle bounding boxes
    - Get UV maps
    - Approximate vertical & horizontal lines with Hough algorithm
    - Map lines with get boxes
    - Discard trivial boxes with IoU
4. Treat every boxes by segments then merge into region (optional)
