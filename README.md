# AI Model Performance Evaluation

This project benchmarks the performance of various AI models, including Falcon 7b, Falcon 40b, Llama 2 7b, Llama 2 13b, Alpaca 13b, Mistral 7b, Vicuna 13b, and Vicuna 30b. Each model was tasked with answering ten questions, and metrics such as time taken, memory used, and energy consumed were recorded for each question. The project was executed on Google Colab using the Pro version to leverage the NVIDIA A100 GPU for the larger models. A Streamlit-based UI was developed to visualize and compare the performance metrics across all models.

## Getting Started

### Prerequisites

To run the project, you will need:
- Access to Google Colab Pro for running the notebooks with A100 GPU.
- Python environment for running the Streamlit application.

### Installation

1. Clone the repository or download the source code.
2. Ensure that your Google Colab environment is set up and that you have access to the Pro version.

### Running the Models

Open the provided Google Colab notebook link:
[Google Colab Notebook](https://colab.research.google.com/drive/138d7ANwVySjYySf9NvGUyWSIv7TrXD82?usp=sharing)

Follow the steps within the notebook to execute the models. The notebook will guide you through the process of running each model, collecting performance data, and saving the results.

### Visualizing the Results with Streamlit

To visualize the performance data:

1. Install Streamlit and other required Python packages:

```sh
pip install streamlit pandas matplotlib numpy

```
Mount your Google Drive to the Colab notebook to access the generated CSV file or download the file and place it in a local directory.

Update the app.py file with the correct path to the CSV file located in the 'final submission' folder.

Run the Streamlit app:

streamlit run app.py

The Streamlit UI will display bar charts comparing the average energy consumed (+ standard deviation), average time taken (+ standard deviation), and average memory used for each model.

Report Section
To view the detailed report of the model performance:

Navigate to the 'Report' section within the Streamlit application.
Follow the instructions provided in the app to interact with the visualizations and interpret the results.
Data Format
The CSV file containing model performance should have the following columns:

Model Name
Average Time Taken + Std Dev
Average Energy Consumed + Std Dev
Average Memory Used
Ensure that the CSV file follows this structure for the Streamlit app to function correctly.
