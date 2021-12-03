# Hierarchical Geo Clustering 



This file will become your README and also the index of your documentation.

## Install

`pip install your_project_name`

## How to use

Fill me in please! Don't forget code examples:

```python
Hier_geo_clus= TreeClusters(3)
Hier_geo_clus.populate_tree(number_per_cluster=200)
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    /tmp/ipykernel_3163093/921516667.py in <module>
          1 Hier_geo_clus= TreeClusters(3)
    ----> 2 Hier_geo_clus.populate_tree(number_per_cluster=200)
    

    /Partition1/Cgeo/git/HierarchicalGeoClustering/HierarchicalGeoClustering/TreeClusters.py in populate_tree(self, number_per_cluster, density_init, factor_density, density_init_list, **kwargs)
        847                 n_childs = random.randint(0, 5)
        848                 node_childs = [
    --> 849                     NodeCluster(name = prev.name +'_'+level_str+str(level)+'_'+node_str+str(i),
        850                                 parent=prev) for i in  range(n_childs)
        851                             ]


    NameError: name 'np' is not defined


tree_original= tree_clusters(4)
tree_original.populate_tree(number_per_cluster=500)
tree_original_points= tree_original.get_points_tree()
X_2=np.array([[p.x,p.y] for p in tree_original_points])
dic_points={'points':[X_2], 'parent':''}
