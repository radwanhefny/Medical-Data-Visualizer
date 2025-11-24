# 📊 Medical-Data-Visualizer
A Python program that analyzes medical examination data and visualizes it using categorical bar plots and a correlation heatmap. The project computes derived features like overweight, normalizes cholesterol and glucose, and provides insights into cardiovascular health trends.

## ✨ Features
- Computes a new `overweight` feature based on BMI.
- Normalizes `cholesterol` and `gluc` values to binary (0 = normal, 1 = above normal).
- Draws categorical bar plots for variables: cholesterol, gluc, smoke, alcohol, activity, overweight.
- Draws a correlation heatmap for the dataset after cleaning.
- Saves all plots as PNG images.

## 📋 Prerequisites
Before running this project, ensure you have:
- Python 3.8+
- Pandas, NumPy, Matplotlib, Seaborn libraries
- CSV dataset `medical_examination.csv` inside a `data` folder
- Basic knowledge of Python and data visualization

## 🚀 Getting Started
1. Clone the repository:
```bash
git clone https://github.com/your-username/Medical-Data-Visualizer.git
cd Medical-Data-Visualizer
```
2. Install dependencies:
```bash
pip install -r requirements.txt
```
3. Run the project:
```bash
python main.py
```
## 🎬 Screenshots / Demo

### Categorical Plot
| Figure | Result |
|--------|--------|
| ![Figure 1](https://github.com/radwanhefny/Medical-Data-Visualizer/raw/main/examples/Figure_1.png) | ![Result 1](https://github.com/radwanhefny/Medical-Data-Visualizer/raw/main/examples/Result_1.png) |

### Heatmap
| Figure | Result |
|--------|--------|
| ![Figure 2](https://github.com/radwanhefny/Medical-Data-Visualizer/raw/main/examples/Figure_2.png) | ![Result 2](https://github.com/radwanhefny/Medical-Data-Visualizer/raw/main/examples/Result_2.png) |




## 🗂️ Project Structure
```
📁 Medical-Data-Visualizer
├── main.py
├── medical_data_visualizer.py   # Core calculations and plotting
├── data/
│   └── medical_examination.csv    # Dataset
├── examples/
│   ├── Figure_1.png
│   ├── Figure_2.png
│   ├── Result_1.png
│   └── Result_2.png
├── requirements.txt
├── test_module.py
└── README.md



```
## 🛠️ Usage
Example usage inside Python:
```python
from medical_data_visualizer import draw_cat_plot, draw_heat_map

cat_fig = draw_cat_plot()
cat_fig.show()

heat_fig = draw_heat_map()
heat_fig.show()


```
Expected output:
- catplot.png → Categorical bar plot for variables by cardio condition
- heatmap.png → Correlation heatmap for cleaned dataset
## ✅ Tests
Run the FreeCodeCamp test suite:
```bash
python test_module.py
```
## 🧠 How It Works
1. Reads the CSV dataset using Pandas.
2. Computes overweight from BMI, normalizes cholesterol and glucose.
3. Generates a categorical plot grouped by cardiovascular condition.
4. Cleans data, computes correlations, and creates a heatmap.
5. Saves both plots as PNG images for reporting or analysis.

## 🤝 Contributing
Contributions are welcome!
1. Fork the repository
2. Create a new feature branch
3. Submit a pull request
Please ensure your code is clean, structured, and well-commented.
## 📝 License
This project is licensed under the MIT license - see the LICENSE file for details. 
## 📞 Support
If you have questions or need help, feel free to:
- Open an issue on this repository  
- Connect with me on LinkedIn: https://www.linkedin.com/in/radwanhefny  
