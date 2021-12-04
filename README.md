# Hierarchical Geo Clustering 



This file will become your README and also the index of your documentation.

## Install

`pip install your_project_name`

## How to use

Fill me in please! Don't forget code examples:

```python
Hier_geo_clus= TreeClusters(3, random_state=1)
```

```python
Hier_geo_clus.populate_tree(number_per_cluster=100, verbose= True)
```

    


```python
Hier_geo_clus.print_structure()
```

    Root
    Root    


```python
Hier_geo_clus.populate_tree(number_per_cluster=200, avoid_intersec= True, verbose= True)
```

    


```python
Hier_geo_clus.root.polygon_cluster
```




![svg](docs/images/output_9_0.svg)



```python
Hier_geo_clus.get_deepth()
```




    4



```python
Hier_geo_clus.root.children
```




    ()



tree_original= tree_clusters(4)
tree_original.populate_tree(number_per_cluster=500)
tree_original_points= tree_original.get_points_tree()
X_2=np.array([[p.x,p.y] for p in tree_original_points])
dic_points={'points':[X_2], 'parent':''}
