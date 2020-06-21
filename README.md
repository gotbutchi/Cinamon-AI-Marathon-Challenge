# Cinamon-AI-Marathon-Challenge
Handwiritng OCR for Vietnamese Address

## Problem Statement: 
Given an image of a handwritten line, participants are required to create an OCR model to transcribe the image into text.
![alt text](https://github.com/gotbutchi/Cinamon-AI-Marathon-Challenge/blob/master/problem_img.png?raw=true)

## Evaluation Metrics
Evaluation is based on Character Error Rate (CER):
  - CER is calculated based on Edit distance (or Levenshtein distance)
  - Given a predicted string A, and the ground truth string B, CER is specified by: $$CER_{A,B} = \frac{Levenshtein(A,B)}{max(len(A), len(B)}$$
  Evaluation is based on character error rate (CER): $$ CER = \left( \sum_{i} CER_{A_{i}, B_{i} \right) $$

## The Method:
For this dataset, I used OpenCV to resize all images into the same height of min_height: for width we apply padding horizontally following the new max width of resized images.

## The result:
Metrics:
- Character Error Rate: 0.10754718033277248
- Word Error Rate:      0.2622086247086247
- Sequence Error Rate:  0.7
