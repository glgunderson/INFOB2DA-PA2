# INFOB2DA-PA2

Group 7 project for INFOB2DA.

---

## Open in Google Colab
Click the badge below to open the main notebook directly in Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/glgunderson/INFOB2DA-PA2/blob/main/notebooks/PA2.ipynb)

---

## Repository Structure
- `data/` → dataset(s)  
- `notebooks/PA2.ipynb` → main project notebook  
- `notebooks/README.md` → placeholder readme for notebooks folder  

---

## Dataset
The dataset is stored in `/data/online_shoppers_intention.csv`.

In Colab, load it directly from GitHub with:

```python
import pandas as pd

url = "https://raw.githubusercontent.com/glgunderson/INFOB2DA-PA2/main/data/online_shoppers_intention.csv"
df = pd.read_csv(url)
print("Dataset loaded, shape:", df.shape)
df.head()

# Collaboration Workflow

To keep collaboration smooth and avoid overwriting each other’s work, follow this process:

1. **Open the notebook in Colab**
   - Use the Colab badge at the top of this README.
   - This ensures everyone is running the same version from GitHub.

2. **Work in a personal branch**
   - In Colab, go to `File → Save a copy in GitHub`.
   - Save your edits to a **new branch** (e.g., `grace-edits`, `teammate1-eda`, `modeling-branch`).
   - Add a clear commit message describing your changes.

3. **Keep outputs clean**
   - Before saving: `Edit → Clear all outputs` in Colab.
   - This prevents giant JSON diffs when committing notebooks.

4. **Open a Pull Request (PR)**
   - On GitHub, open a PR from your branch into `main`.
   - Teammates can review changes before merging.

5. **Merge carefully**
   - Only merge notebooks that run cleanly from start to finish (`Runtime → Run all` in Colab).
   - Resolve any conflicts before merging into `main`.

---

### 🔹 Best Practices
- One person per branch = no stepping on toes.
- Always load the dataset using the GitHub raw link (see Dataset section).
- Use clear commit messages (e.g., `Added revenue visualization`, not just `Update`).
- Test your notebook fully (`Runtime → Run all`) before opening a PR.
