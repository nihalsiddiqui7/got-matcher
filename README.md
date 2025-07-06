# 🧝‍♂️ Game of Thrones Character Matcher

Ever wondered which Game of Thrones character speaks most like another?  
This Streamlit app analyzes the **word usage patterns of top 25 characters** from the show and finds the most similar character based on their dialogue!

> ⚔️ Built with data science, powered by `t-SNE`, and wrapped in a beautiful Streamlit interface.

---

## 🚀 Live Demo

🔗 [Launch the App](https://your-streamlit-link.streamlit.app)

---

## 🧠 What This App Does

- Takes your selected **Game of Thrones character**
- Analyzes their dialogue from the show
- Uses **t-SNE** (t-distributed stochastic neighbor embedding) to reduce high-dimensional word vector data into 2D
- Finds and displays the **closest-matching character** in the embedded space
- Shows **side-by-side portraits** and number of words spoken

---

## 🗂 Tech Stack

| Tool | Usage |
|------|-------|
| `pandas` | Load and process character dialogue |
| `numpy` | Math for distance calculations |
| `t-SNE` (`sklearn.manifold.TSNE`) | Dimensionality reduction for visual clustering |
| `streamlit` | Build the interactive web app |
| `duckduckgo-search` / `SerpAPI` | Download character portraits |
| `urllib.request` | Image downloads |
| `matplotlib` (optional) | Embedding visualization |
| `scikit-learn` | t-SNE + utilities |

---

## 📁 Project Structure

got-matcher/
├── app.py # Main Streamlit app
├── prepare_data.py # Script to build character word data & embeddings
├── download_images.py # Downloads top 25 portraits
├── data/
│ └── top_25_characters.csv
├── images/
│ └── tyrion_lannister.jpg, ...
├── requirements.txt
├── README.md




## 📦 Installation (Local)

1. Clone the repo:

```bash
git clone https://github.com/yourusername/got-matcher.git
cd got-matcher

pip install -r requirements.txt


streamlit run app.py
