# Data Science Tutorial Setup Guide

This guide will help you set up your environment to run the data science tutorial notebook (`data_science_tutorial.ipynb`).

## Installing Python

### For macOS:
1. Visit the official Python website: https://www.python.org/downloads/
2. Click on "Download Python" (latest version recommended)
3. Run the downloaded installer package
4. Follow the installation wizard instructions
5. Verify installation by opening Terminal and typing:
   ```bash
   python3 --version
   ```

### For Windows:
1. Visit the official Python website: https://www.python.org/downloads/
2. Click on "Download Python" (latest version recommended)
3. Run the downloaded installer
4. **Important**: Check the box that says "Add Python to PATH" during installation
5. Follow the installation wizard instructions
6. Verify installation by opening Command Prompt and typing:
   ```bash
   python --version
   ```

## Installing Dependencies

This project uses several Python packages for data science and machine learning. You can install all required dependencies at once using the provided `requirements.txt` file:

1. Open Terminal (macOS) or Command Prompt (Windows)
2. Navigate to the project directory:
   ```bash
   cd path/to/your/project
   ```
3. Install all dependencies using pip:
   ```bash
   pip install -r requirements.txt
   ```

This will install the following packages:
- numpy: For numerical computing
- pandas: For data manipulation and analysis
- matplotlib: For creating static visualizations
- seaborn: For enhanced statistical visualizations
- scikit-learn: For machine learning algorithms
- jupyter: For running Jupyter notebooks
- notebook: For the Jupyter notebook interface
- ipykernel: For Python kernel support in Jupyter

## Installing Jupyter Notebook

Once Python is installed, you can install Jupyter Notebook using pip (Python's package installer):

1. Open Terminal (macOS) or Command Prompt (Windows)
2. Install Jupyter Notebook by running:
   ```bash
   pip install notebook
   ```
3. Verify the installation by running:
   ```bash
   jupyter --version
   ```

## Running the Tutorial Notebook

### Download the Dataset
Before running the notebook, you'll need to download the synthetic healthcare dataset:

1. Visit [Synthea Synthetic Health Data Downloads](https://synthea.mitre.org/downloads)
2. Download the "10k Sample Synthetic Patient Records, CSV Format"
3. Extract the downloaded file - it will create a directory named `10k_synthea_covid19_csv` containing all the CSV files
4. Move the extracted `10k_synthea_covid19_csv` directory into your project folder

Note: This dataset contains synthetic (artificially generated) patient data created by the MITRE Corporation's Synthea tool. It's designed to simulate realistic but non-real patient health records for educational and development purposes. No real patient data is included.

### Running the Notebook
1. Open Terminal (macOS) or Command Prompt (Windows)
2. Navigate to the project directory:
   ```bash
   cd path/to/your/project
   ```
3. Start Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
4. Your default web browser will open with the Jupyter Notebook interface
5. Click on `data_science_tutorial.ipynb` to open the tutorial notebook
6. To run cells in the notebook:
   - Click the "Run" button in the toolbar
   - Or use the keyboard shortcut: Shift + Enter
   - To run all cells: Cell → Run All

## Additional Tips

- To stop the Jupyter Notebook server, press Ctrl + C in the terminal
- If you encounter any permission issues, you might need to run the installation commands with `sudo` on macOS
- Make sure you have a stable internet connection as some packages might need to be downloaded during the tutorial

## Troubleshooting

If you encounter any issues:

1. Make sure Python is properly installed and added to PATH
2. Try updating pip:
   ```bash
   python -m pip install --upgrade pip
   ```
3. If Jupyter Notebook fails to start, try reinstalling:
   ```bash
   pip uninstall notebook
   pip install notebook
   ```

### Alternative Installation Guide

If you're having trouble with the Python installation, you can refer to the comprehensive installation guide from Cornell University's CS1110 course:
[Cornell CS1110 Python Installation Guide](https://www.cs.cornell.edu/courses/cs1110/2024fa/materials/python/)

This guide provides detailed, platform-specific instructions for installing Python and includes additional troubleshooting steps that might be helpful.

For additional help, please refer to the official documentation:
- Python: https://docs.python.org/3/
- Jupyter Notebook: https://jupyter.org/documentation 