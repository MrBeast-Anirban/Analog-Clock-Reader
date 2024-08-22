A model capable of accurately detecting the time displayed on an analog clock, regardless of its orientation or angle. The model is robust enough to handle variations in lighting conditions, clock design, and background clutter. It accurately identifies the position of the clock hands and translate their positions into a digital time format.

<h3>Dataset used :-</h3> https://www.kaggle.com/datasets/gpiosenka/time-image-datasetclassification

<h3>Approach Used :-</h3>  
<h4>1. Classic Computer Vision Approach</h4>
   Analog clock reading, a quintessential task in computer vision, relies on a set of traditional techniques to accurately interpret the positions of hour and minute hands. These techniques leverage fundamental principles of image processing and object detection to discern the temporal information represented by the clock’s analog display.Some of the techniques include Thresholding, Contour Detection, Contour Sorting and Drawing, Image Thinning, Circle Detection, etc. But it struggles and performs bad with real life situations
bad Lighting, angle of clock placement and overexposure of graphical orientation on clock face.

<h4>3. CNN on a large clock face dataset (linked above)</h4>
  Implementing Convolutional Neural Networks (CNNs) for analog clock reading offers a promising approach to overcome the limitations of traditional computer vision techniques, particularly in handling real‑world scenarios with skewed or tilted clock Images somewhat only if the model is trained with similar kid of clock image but sadly this dataset contains only front facing images which leads to our next approach.

<h4>3. CNN with Synthetic Clock Generator</h4>
  To generate a dataset, we employ a Synthetic Clock Generator to produce input images depicting conical clocks and their corresponding "homographic images". These homographic images simulate distortions such as tilting, slanting, or skewing that might occur when viewing clocks from non‑standard angles or orientations. This enables the model to learn how to accurately detect clock hands despite variations in orientation or perspective.
   
