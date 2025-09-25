# iSCMS Hackathon 2025: Mass Spectrum Signal Processing for Noise Reduction

We are excited to announce our upcoming hackathon!  
**Date:** September 25th  
**Time:** 12:00 PM – 5:00 PM Central Time  

- Zoom Link: [https://uic.zoom.us/j/7180490853?omn=84858766470](https://uic.zoom.us/j/7180490853?omn=84858766470)
- Zoom Meeting ID: `718 049 0853`

To help participants around the world, here are some common conversions:
- 1:00 PM – 6:00 PM Eastern Time (ET)  
- 10:00 AM – 3:00 PM Pacific Time (PT)  
- 5:00 PM – 10:00 PM Greenwich Mean Time (GMT/UTC)  
- 7:00 PM – 12:00 AM Central European Time (CET)  

## Task at Hand
The challenge for this hackathon is:  
**Mass spectrum signal processing for noise reduction.**  

Participants will work on designing and implementing approaches to clean noisy spectra, improving the accuracy and interpretability of downstream analyses.

---

## Instructions

We provide three csv files containing mass spectra with noise and true signal. 
- train.csv
- validation.csv
- test.csv

The CSV files are in the following format:
- `spec_no`: A non-unique index respresenting the spectrum. For example, each row with spec_no = 1 will correspond to all the peaks to that spectrum.
- `mz`: The m/z value for a signal
- `intensity`: The intensity value for a signal
- `signal`: A binary label representing if the peak is true signal (signal = 1) or noise (signal = 0)

The **train set** contains **600 labeled spectra** and the **validation set** contains **100 labeled spectra**.

The test set ***does not contain labels***. We will use this set to evalauate your solution.

### Submission Instructions
1. Annotate **test.csv** by adding another column, signal, with binary values either 0 or 1. 
- *Ensure that you do not change the length of this file!* Do not remove peaks or spectra before submission. If you believe a peak is noise, label this with signal = 0.
2. Navigate to http://pepchem.org:35098/submit
3. Fill out the form with your information and upload *your annotated test.csv* file in the "File Upload" section.
4. View you result at http://pepchem.org:35098/ranking

## Rules
1. **Open Source Requirement**  
   - All submitted code must be open source. While code submission is not required within the time frame of the hackathon, you must be willing to share your solution in our joint effort.

2. **Publication Commitment**  
   - We aim to combine the best efforts into a joint publication.  
   - By participating, you agree to potentially contribute additional time *after* the hackathon to help prepare your work for publication.  

3. **Resource Usage**  
   - You may use any computational resources available to you (local machines, HPC systems, cloud platforms, etc.).

      - However, your final solution must be runnable on a modern high-end personal computer. Avoid approaches that demand excessive memory or compute.

      - For example, it is acceptable to train a model on a GPU cluster, but the resulting model should still be able to run inference efficiently on a personal computer.

---
