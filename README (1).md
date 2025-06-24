# Optimization Knowledge Management

This project is a demo application for identifying and evaluating the similarity between mathematical functions or datasets using user-provided inputs. It is built using Streamlit and provides an interactive interface for working with optimization functions, their characteristics, and their outputs.

## Features

- Input a custom function expression for similarity comparison.
- Upload data points via list or Excel file.
- Use characteristics (e.g., convexity, separability) to query a function database.
- Compare function similarity using cosine similarity of normalized sample outputs.
- Retrieve matching functions from a MongoDB database.
- Perform symbolic regression and neural network-based optimization.
- Visual feedback for best match and predicted solution values.

## Usage

1. Run the app:
   ```bash
   streamlit run OptKM_demo.py
   ```

2. Choose your input type:
   - Function Expression
   - Data Points (list or Excel)
   - Function Characteristics

3. View the best matching function based on cosine similarity.

4. Optionally proceed to symbolic regression or prediction using neural networks.

## Requirements

Install dependencies using the `requirements.txt` file:
```bash
pip install -r requirements.txt
```

## Configuration

The app connects to a MongoDB Atlas instance:
- Update the MongoDB URI in `OptKM_demo.py` if needed.
- It queries `SiemensWork.CleanFunctions` for function metadata and `SiemensWork.Models` for pretrained weights.

## Security Note

Ensure sensitive credentials such as API keys and MongoDB URIs are securely handled. Avoid hardcoding them in production environments.

---

## Author

Project by **Optimization Knowledge Management** team.
