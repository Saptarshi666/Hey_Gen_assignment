# Hey Gen At-Home Assignment

This repository contains the Hey Gen at-home assignment as provided by **David Steffes**.

---

## Input

The `input` folder contains:
1. **A video**: This video, sourced from YouTube, involves considerable and constant POV shifts between multiple individuals.
2. **A reference image**: The reference image corresponds to the individual whose face we aim to track in the video.

---

## Output

The program generates the following in the output directory:
1. **`metadata.json`**: This file adheres to the format specified in the assignment requirements.
2. **`clips` folder**: Contains small video clips of the individual when they appear in the input video. Due to near-constant POV shifts, some clips may be as short as 0 seconds.
3. **`images` folder**: Contains all images of the individual extracted from these clips. Note that the images are small in size and may require zooming in to view properly.

---

## Program Overview

The program is written in a **Python notebook** and executed on Kaggle.

### Notebook Structure

1. **Cell 1**: Default Kaggle-generated cell. Can be skipped.
2. **Cell 2**: Imports all required libraries.
3. **Cell 3**: Contains the main functions that perform video processing, face tracking, and output generation.
4. **Cell 4**: Defines variables for:
   - Input video path
   - Input image path
   - Output directory path  
   Calls the functions from Cell 3 for execution.  

5. **Remaining Cells**: Primarily address Kaggle-specific issues, such as:
   - Loading files into a folder.
   - Converting output folders into zip files for download.  
   These cells can be ignored if not running on Kaggle.

---

## Execution Instructions

To execute the notebook:
1. Update the variables in **Cell 4** with paths to your:
   - Input video
   - Input image
   - Desired output directory
2. Run the notebook cells sequentially.

### Output Directory Structure

After execution:
- All **images** will be saved in the `images` folder.
- All **video clips** will be stored directly in the output directory (not in the `images` folder).
- The `metadata.json` file will also be available directly in the output directory.
