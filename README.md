# PSD Parser & Creator

## Overview

This project provides Python scripts to manipulate Adobe Photoshop files (PSD). It enables you to:

  * Parse PSD files by extracting their layers and saving them as PNG images.

  * Rebuild PSD files from multiple PNG images, effectively reversing the parsing process.

## Project Structure

* parser.py
  - Parses a PSD file into individual PNG layers.

  - Rebuilds a PSD file from extracted PNGs.

  - Saves both the layered PSD and a merged PNG preview.

* utils.py
  
Contains helper functions:

  parse_file(psdFile, pngFile, parseOutFolder) : Extracts layers from a PSD and saves them as PNGs.
     
  load_images(imgPath, files) : Loads PNG images into memory as RGBA.
     
  images_to_layers(psd, images, lefttop) : Adds images as layers to a PSD file.
     
  set_opacity_blend_mode(psd) : Adjusts opacity and blend mode of layers.
     
  image_to_psd(image_obj, save_path) : Converts a PIL image into a PSD file with a visible layer.

## Prerequisites

   Ubuntu 18

   Python 3.8

   Libraries: PIL (Python Imaging Library), psd-tools

## Usage
``` bash
python parser.py

