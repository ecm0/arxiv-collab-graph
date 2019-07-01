# Collaboration graph from Arxiv paper co-authoring

This notebook shows how to generate a collaboration graph from Arxiv metadata.

The collaboration graph describes relationships between researchers in a scientific field. The relationship is established based on co-authorship of publications stored in the Arxiv preprint server.

The graph nodes are researchers, and the graph edges connect two researchers that have co-authored at least one publication.

The graph is stored in a GML file, and it can be visualize with a graph drawing tool such as Gephi or others (see e.g., https://networkx.github.io/documentation/stable/reference/drawing.html).

This demonstration is specialized to the field of gravitational-wave astronomy, based on the gr-qc e-print category, but it can be applied to any category.

Arxiv metadata can be accessed at:

``` R. Stuart Geiger (2019). "ArXiV Archive: A Tidy and Complete Archive of Metadata for Papers on arxiv.org." Zenodo. http://doi.org/10.5281/zenodo.1463242  ```

This repo includes a local copy of the Arxiv metadata for the gr-qc category.

# Installation instructions

```python3 -m venv arxiv_proc
source arxiv-proc/bin/activate
pip install nameparser
pip install pandas
pip install networkx
pip install matplotlib
pip install pip setuptools --upgrade
ipython kernel install --user --name=arxiv-proc
```
