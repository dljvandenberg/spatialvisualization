# Spatial Visualization

## Install

```
conda create -n spatial python=3
conda activate spatial
pip install -r requirements.txt
```

Notes:

- geopandas installation can be checked using: `import geopandas as gpd`
    - On Mac OSX, some issues have been observed with the fiona dependency when installing geopandas:
        `ImportError: dlopen( .. /fiona/ogrext.cpython-36m-darwin.so, 2): Symbol not found: _sqlite3_column_table_name`
    - Which can be solved by downgrading fiona (https://github.com/Toblerity/Fiona/issues/588):
        `pip install fiona==1.7.11.post1`


## Run

```
conda activate spatial
jupyter-notebook
```