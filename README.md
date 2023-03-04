# Petroglyph Detection
Detecting petroglyphs in an image using YOLOv5 object detection model.  
This Colab notebook loads a pre-trained YOLOv5 model and predicts bounding boxes for images of petroglyphs. Trained on a custom dataset of 1,000 images of petroglyph, annotated with bounding boxes by me. The model was trained using the YOLOv5 tutorial notebook found [here](https://colab.research.google.com/github/ultralytics/yolov5/blob/master/tutorial.ipynb).  

## Acknowledgment of Bias
This project is intended only as a learning experience in computer vision, not as an academic work. A major source of bias in this project comes from the annotation process, which was performed by a hobbyist (me) with no understanding of the meaning of these symbols. Several thousand images were downloaded from Flickr, which the annotator inspected for glyphs and arbitrarily decided whether or not to label. Some images showed panels with hundreds of individual glyphs; some images showed densely interconnected patterns from which individual glyphs could not be distinguished; many contained isolated dots lines or splotches; all of which the annotator simply ignored. The overarching assumption was that petroglyphs are made of distinct symbols, like words, and that each individual symbol can be delimited by being surrounded by space - thus easily placed within a bounding box. But the annotator immediately found hundreds of instances that proved the naivety of this assumption, and instead settled for just labeling images with clearly defined symbols.

<img src="./github_preview_images/example_images/27915781308.jpg" style="width: 40%;"><img src="./github_preview_images/example_predictions/27915781308.jpg" style="width: 40%;">

<img src="./github_preview_images/example_images/28760741518.jpg" style="width: 40%;"><img src="./github_preview_images/example_predictions/28760741518.jpg" style="width: 40%;">

<img src="./github_preview_images/example_images/30359780592.jpg" style="width: 40%;"><img src="./github_preview_images/example_predictions/30359780592.jpg" style="width: 40%;">

<img src="./github_preview_images/example_images/6183174382.jpg" style="width: 40%;"><img src="./github_preview_images/example_predictions/6183174382.jpg" style="width: 40%;">

<img src="./github_preview_images/example_images/panel.jpg" style="width: 40%;"><img src="./github_preview_images/example_predictions/panel.jpg" style="width: 40%;">

