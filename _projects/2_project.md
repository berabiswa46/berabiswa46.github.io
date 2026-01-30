---
layout: page
title: Autonomous Vehicle Perception
description: Vision systems for self-driving cars and intelligent transportation
img: assets/img/projects/autonomous.jpg
importance: 2
category: ongoing
---

## Project Overview

Developing robust computer vision algorithms for autonomous vehicles that can perceive and understand complex driving environments in real-time. Our system handles object detection, lane detection, traffic sign recognition, and scene understanding under various weather and lighting conditions.

### Key Components

1. **Multi-Object Detection & Tracking**
   - Real-time detection of vehicles, pedestrians, cyclists, and obstacles
   - Temporal tracking across video frames
   - Prediction of object trajectories

2. **Lane Detection & Road Segmentation**
   - Accurate lane boundary detection
   - Drivable area segmentation
   - Road marking recognition

3. **Traffic Sign & Signal Recognition**
   - Detection and classification of traffic signs
   - Traffic light state recognition
   - Road condition assessment

4. **Adverse Condition Handling**
   - Robust performance in rain, fog, and low-light conditions
   - Multi-sensor fusion (camera + LiDAR + radar)
   - Weather-adaptive algorithms

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/av1.jpg" title="object detection" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/av2.jpg" title="lane detection" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: Multi-object detection and tracking. Right: Lane and road segmentation.
</div>

### Technical Highlights

- **Real-time Processing**: Achieving 30+ FPS on embedded GPU platforms
- **High Accuracy**: 98% precision on KITTI benchmark dataset
- **Efficient Architecture**: Optimized neural networks for edge deployment
- **Safety Critical**: Extensive testing and validation protocols

### Partnerships

- Automotive Industry Partner: [Company Name]
- Testing Facility: [Location] Autonomous Driving Test Track
- Data Collection: 10,000+ hours of annotated driving footage

### Funding

- Department of Transportation Grant: $1.2M
- Industry Partnership: $800K
- University Research Fund: $200K

**Timeline**: March 2024 - March 2027

**Status**: <span style="background: #28a745; color: white; padding: 4px 12px; border-radius: 4px;">Active</span>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, _bled_ for your project, and then... you reveal its glory in the next row of images.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>

The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}

```html
<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
```

{% endraw %}
