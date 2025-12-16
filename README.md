# 📊 SporeQuant 
## Automated Spore Counting from Hemocytometer Images

SporeQuant is a free, open-source image analysis tool for automated counting of spores, particularly fungal spores, from hemocytometer (Neubauer chamber) microscopy images.
It replaces manual spore counting with a fast, reproducible, and accessible digital workflow.

SporeQuant is implemented in Python and deployed as a Streamlit web application, allowing use directly from a web browser on a computer or smartphone.
The program requires no installation, no specialized hardware, and no programming experience.

**🌐 Live app: https://spore-quant.streamlit.app/**

### Key Features
- Automated spore counting using image thresholding and blob detection
- Real-time parameter tuning with visual feedback
- Optional hemocytometer grid removal
- Manual correction tools for edge cases
- Automatic calculation of spore concentration (spores/mL)
- Batch analysis with replicate averaging
- Fully open-source (GPL-3.0 license)

### Typical Use Case
1. Get a microscopy image of a Neubauer hemocytometer (usually at 40× magnification)
2. Upload the image to SporeQuant
3. Crop to a 0.2 × 0.2 mm counting square
4. Adjust threshold (if needed)
5. Obtain:
   - Spore count
   - Spore concentration (with dilution correction)
   - Annotated output image

### Method Summary
SporeQuant follows a lightweight image-processing pipeline:
1. Image cropping and grayscale conversion
2. Optional grid-line removal
3. Binary thresholding
4. Blob detection with size filtering
5. Spore concentration calculation 

**Using SporeQuant led to a 63% reduction in analysis time compared to manual counting.**

### Citation and Additional Information
For additional information, please see our preprint: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5912070
