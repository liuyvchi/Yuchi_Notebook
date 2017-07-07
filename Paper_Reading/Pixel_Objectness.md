# Pixel Objectness

Two main strategies for generic object segmentation:

- saliency
- object proposal

pixel objectness: a new approach to generic foreground segmentation. Given a novel image, the goal is to determine the likelihood that each pixel is part of a foreground object (as opposed etc.)

## Approach

formulate the task of foreground object segmentation as densely labeling each pixel in the image as either "object" or "background"

input: m * n * c                  output: m * n

the method should: 

1. predict a pixel-level map that aligns well with object boundaries
2. generalize so it can assign high probability to pixels of unseen object categories

#### Mixing explicit and implicit representations of objectness

explicit boundary-level annotations

implicit image-level object category annotations