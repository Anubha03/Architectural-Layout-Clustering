# Design Standardisation for Architectural Layouts

A 2024 DS203 group project at IIT Bombay, guided by **Prof. Vinay Kulkarni**, Centre for Machine Intelligence and Data Science.

## Workflow

- Converts layout bitmaps to grayscale and binary shape representations.
- Extracts flattened image features, explores PCA, and compares clustering settings with inertia and silhouette scores.
- Investigates K-means and DBSCAN for shape-based design families.
- Derives four complexity descriptors: perimeter-to-area ratio, convexity defects, mirror asymmetry, and contour-point count.
- Uses standardized descriptors and PCA for three complexity clusters.
- Retrieves a suitable design family from requested complexity, area, and bounding-box dimensions using centroid distances.

## Recorded findings

The presentation describes **1,183 layouts**, 100 PCA components retaining **98.96%** of variance, and a selected **four-family K-means shape grouping**. Separately, the three complexity clusters contain 628, 381, and 174 layouts. These shape families and complexity categories are different groupings.

## Files and setup

- [Analysis notebook](notebooks/architectural_layout_clustering.ipynb)
- [Group presentation](reports/E7_Architectural_Layouts_Presentation.pdf)

Install dependencies with `pip install -r requirements.txt` and open the notebook using `jupyter lab`. Supply the original layout images in an `Images/` folder relative to the notebook working directory. The image dataset is not included.
