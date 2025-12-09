# ai-delivery-route-planner
An AI-powered delivery route planner that uses search algorithms and constraint satisfaction to find the most efficient delivery paths while obeying constraints such as visiting each location once, avoiding blocked roads, and meeting delivery time windows.

## How to Run

### Prerequisites

- Python 3.7 or higher
- Jupyter Notebook or JupyterLab
- Required Python packages (see Installation below)

### Installation

1. **Clone or download this repository**

2. **Install required packages** using pip:
   ```bash
   pip install pandas numpy matplotlib scikit-learn jupyter
   ```

   Or if you prefer using a virtual environment (recommended):
   ```bash
   # Create virtual environment
   python -m venv venv
   
   # Activate virtual environment
   # On macOS/Linux:
   source venv/bin/activate
   # On Windows:
   venv\Scripts\activate
   
   # Install packages
   pip install pandas numpy matplotlib scikit-learn jupyter
   ```

### Running the Notebook

1. **Ensure the dataset is in place**: Make sure `amazon_delivery.csv` is in the same directory as the notebook.

2. **Start Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```
   Or if using JupyterLab:
   ```bash
   jupyter lab
   ```

3. **Open the notebook**: Navigate to and open `delivery_route_planner.ipynb` in your browser.

4. **Run all cells**: 
   - You can run cells individually by selecting a cell and pressing `Shift + Enter`
   - To run all cells at once, go to `Cell` → `Run All` in the menu bar
   - Or use the keyboard shortcut: `Ctrl + Shift + Enter` (Windows/Linux) or `Cmd + Shift + Enter` (macOS)

### Expected Output

The notebook will:
- Load and explore the Amazon delivery dataset
- Visualize data distributions and geographic locations
- Run search algorithms (BFS, DFS, A*, Greedy) to find optimal routes
- Solve constraint satisfaction problems with time windows
- Train a machine learning model (Random Forest) to predict travel times
- Generate visualizations comparing algorithm performance
- Display route maps and delivery timelines

### Notes

- The notebook processes 8 delivery locations from the Urban area for demonstration
- Execution time varies by algorithm (Greedy is fastest, BFS/DFS are slower but optimal)
- All visualizations will be displayed inline in the notebook
- The ML model training may take a few seconds depending on your system
