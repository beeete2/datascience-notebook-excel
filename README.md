# datascience-notebook-excel

Supported DataFrame.to_excel for datascience-notebook.

## Example
**Run docker container**
```bash
docker run -d --name notebook -p 8888:8888 \
  -v $(pwd):/home/jovyan/work \
  beeete2/datascience-notebook-excel start-notebook.sh --NotebookApp.token=''
```

**Run following code in the cell.**
```python
import pandas as pd
import seaborn as sns
iris = sns.load_dataset("iris")

iris.to_excel('irls.xlsx')
```
then, `irls.xlsx` was output to current directory.
