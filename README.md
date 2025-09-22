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

## Example Submission Workflow

To help you familiarize yourself with the data before the competition, we provide an [example.mzML](https://raw.githubusercontent.com/chrisagrams/iSCMS-Hackathon-2025/refs/heads/main/data/example.mzML) file.  
An mzML file is an open, XML-based standard format for mass spectrometry data. It stores information about spectra, including metadata, mass-to-charge (m/z) values, and intensity measurements.

There are various libraries to parse mzML files for Python and R. One such library for Python is [pymzML](https://pymzml.readthedocs.io/en/latest/).

We also provide an [example_output.csv](https://raw.githubusercontent.com/chrisagrams/iSCMS-Hackathon-2025/refs/heads/main/data/example_output.csv) file with the following structure:

- **spec_no**: Spectrum number (integer).  
- **mz**: Mass-to-charge ratio (floating-point, 64-bit precision).  
- **peak**: Binary label — `0` indicates noise, and `1` indicates a true signal.

We will provide the final mzML file used for the competition at **12:00 PM Central Time on the day of the hackathon**.

We expect your solution to follow the same format as our provided example CSV file, providing your identifications (true signal or nosie) for each peak within the mzML.

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
