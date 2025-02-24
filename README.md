#  Sarcasm Detector Using Embeddings

##  Overview
This project focuses on **building a sarcasm detector** using **word embeddings**. The goal is to **assign numerical values** to words based on their occurrence in **sarcastic or realistic headlines**, allowing us to computationally establish sentiment.

##  How It Works
1. **Encoding Words**  
   - Words from **sarcastic headlines** are assigned **positive values**.
   - Words from **realistic headlines** are assigned **negative values**.
   
2. **Sentiment Scoring**  
   - Given a new sentence, we calculate a **sentiment score** by summing the values of its words.
   - If the score is **positive**, the sentence is likely **sarcastic**.
   - If negative, it's considered **realistic**.

3. **Using Vectors for Context**  
   - The model doesn’t "understand" words directly.
   - Instead, it moves word representations based on sarcasm or realism, forming a **vector space** to determine meaning.

## Repository Structure
- `main.ipynb` - Jupyter Notebook with the implementation and explanations.
- `data/` - Folder containing the sarcasm dataset.
- `models/` - Saved models for sarcasm detection.
- `requirements.txt` - Dependencies to install before running the notebook.

## Getting Started
**Install Dependencies**
```bash
pip install -r requirements.txt
```

**Run the Jupyter Notebook**

```bash
jupyter notebook main.ipynb
```

## Example
**Input** 
```python
"neutered male named against germany, wins statuette!"
```

**Output**

```ini
Score = 2 → Sarcastic Sentence
```

## License
This project is open-source under the MIT License.