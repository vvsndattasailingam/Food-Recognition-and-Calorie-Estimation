## Food Recognition and Calorie Estimation

This project estimates the calories of food items using image processing techniques. It involves segmenting the food region, calculating area, and performing related analysis.

---

### Folder Structure

- **`input_images`**: Contains the input images for the project.
- **`sample_outputs_of_onion`**: Contains sample output images from the code for testing purposes.
- **`Food_Calories_Estimation_Using_Image_Processing.ipynb`**: The main code file implementing the food recognition and calorie estimation.
- **`README.md`**: Documentation file.
- **`requirements.txt`**: File specifying the required Python libraries.

---

### Installation

To set up the project environment, install the following dependencies:

1. Clone the repository or download the files.
2. Install the required libraries:

   ```bash
   pip install -r requirements.txt
   ```

   Alternatively, run the following command to install the essential packages:

   ```bash
   pip install opencv-python numpy tflearn
   ```

3. Ensure you have Python 3.7+ installed.

---

### Configuration Instructions

#### Google Colab Setup

1. Open the `.ipynb` file in Google Colab.
2. Mount your Google Drive to access the input files and save output files:

   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```

#### Local Setup

1. Place your input images in the `input_images` folder.
2. Ensure the output directory exists for storing results. If not, the script will create it automatically.
3. Update the paths in the code cells to reflect your local environment, e.g.,

   ```python
   data = os.path.join(os.getcwd(), "input_images")
   ```

---

### Usage Instructions

1. Upload the `.ipynb` file to Google Colab or open it locally in Jupyter Notebook.
2. Upload the input files (images) to the `input_images` folder or a path of your choice.
3. Update paths in the notebook code to match the location of your images.
4. Run the cells sequentially to process the images and calculate calorie estimates.
5. Output images will be saved in the directory specified in the code.

---

### Sample Workflow

#### Food Area Calculation:

1. The `getAreaOfFood` function segments the food from the background.
2. Output images at different processing stages are saved for reference.
3. The calculated food area and other features are used for calorie estimation.

#### Output Files:

- Processed images showing different stages of segmentation.
- Final result images highlighting the detected food.

---

### Software and Hardware Requirements

- **Software**: Python 3.7+, Jupyter Notebook/Google Colab
- **Libraries**: OpenCV, NumPy, TFLearn
- **Hardware**: Minimum 12GB RAM (for Colab)

---

### Special Instructions

- Upload input files to Google Drive or your local directory.
- Update paths in the notebook code to reflect the correct file locations.
- Use high-resolution images for better accuracy.

Feel free to contribute and enhance this project!
