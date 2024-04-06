# Comparing `tmp/pcg_skel-0.3.5.tar.gz` & `tmp/pcg_skel-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcg_skel-0.3.5.tar", last modified: Fri Jan  5 03:03:11 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pcg_skel-0.3.5.tar` & `pcg_skel-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,14 @@
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-01-05 03:03:11.496416 pcg_skel-0.3.5/
--rw-r--r--   0 caseysm    (501) staff       (20)     1842 2022-11-15 01:01:33.000000 pcg_skel-0.3.5/LICENSE.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       24 2022-11-15 01:01:33.000000 pcg_skel-0.3.5/MANIFEST.in
--rw-r--r--   0 caseysm    (501) staff       (20)    10542 2024-01-05 03:03:11.496137 pcg_skel-0.3.5/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)     9986 2024-01-05 03:01:22.000000 pcg_skel-0.3.5/README.md
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-01-05 03:03:11.494650 pcg_skel-0.3.5/pcg_skel/
--rw-r--r--   0 caseysm    (501) staff       (20)      117 2024-01-05 03:02:57.000000 pcg_skel-0.3.5/pcg_skel/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)     1926 2022-11-15 01:01:33.000000 pcg_skel-0.3.5/pcg_skel/chunk_cache.py
--rw-r--r--   0 caseysm    (501) staff       (20)    15443 2023-07-23 12:06:57.000000 pcg_skel-0.3.5/pcg_skel/chunk_tools.py
--rw-r--r--   0 caseysm    (501) staff       (20)    11760 2023-04-21 18:23:20.000000 pcg_skel-0.3.5/pcg_skel/features.py
--rw-r--r--   0 caseysm    (501) staff       (20)    25012 2023-03-07 01:08:41.000000 pcg_skel-0.3.5/pcg_skel/nocache.py
--rw-r--r--   0 caseysm    (501) staff       (20)     6228 2023-07-13 17:39:53.000000 pcg_skel-0.3.5/pcg_skel/pcg_anno.py
--rw-r--r--   0 caseysm    (501) staff       (20)    36782 2023-04-21 20:14:20.000000 pcg_skel-0.3.5/pcg_skel/pcg_skel.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3216 2022-11-15 01:01:33.000000 pcg_skel-0.3.5/pcg_skel/skel_utils.py
--rw-r--r--   0 caseysm    (501) staff       (20)     2866 2023-03-07 01:08:41.000000 pcg_skel-0.3.5/pcg_skel/utils.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-01-05 03:03:11.495867 pcg_skel-0.3.5/pcg_skel.egg-info/
--rw-r--r--   0 caseysm    (501) staff       (20)    10542 2024-01-05 03:03:11.000000 pcg_skel-0.3.5/pcg_skel.egg-info/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)      411 2024-01-05 03:03:11.000000 pcg_skel-0.3.5/pcg_skel.egg-info/SOURCES.txt
--rw-r--r--   0 caseysm    (501) staff       (20)        1 2024-01-05 03:03:11.000000 pcg_skel-0.3.5/pcg_skel.egg-info/dependency_links.txt
--rw-r--r--   0 caseysm    (501) staff       (20)      112 2024-01-05 03:03:11.000000 pcg_skel-0.3.5/pcg_skel.egg-info/requires.txt
--rw-r--r--   0 caseysm    (501) staff       (20)        9 2024-01-05 03:03:11.000000 pcg_skel-0.3.5/pcg_skel.egg-info/top_level.txt
--rw-r--r--   0 caseysm    (501) staff       (20)      112 2022-11-15 01:01:33.000000 pcg_skel-0.3.5/requirements.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       38 2024-01-05 03:03:11.496512 pcg_skel-0.3.5/setup.cfg
--rw-r--r--   0 caseysm    (501) staff       (20)     1467 2022-11-15 01:01:33.000000 pcg_skel-0.3.5/setup.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pcg_skel-1.0.0/pcg_skel/__init__.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 pcg_skel-1.0.0/pcg_skel/chunk_cache.py
+-rw-r--r--   0        0        0    15432 2020-02-02 00:00:00.000000 pcg_skel-1.0.0/pcg_skel/chunk_tools.py
+-rw-r--r--   0        0        0    13033 2020-02-02 00:00:00.000000 pcg_skel-1.0.0/pcg_skel/features.py
+-rw-r--r--   0        0        0    23437 2020-02-02 00:00:00.000000 pcg_skel-1.0.0/pcg_skel/nocache.py
+-rw-r--r--   0        0        0     8017 2020-02-02 00:00:00.000000 pcg_skel-1.0.0/pcg_skel/pcg_anno.py
+-rw-r--r--   0        0        0    24327 2020-02-02 00:00:00.000000 pcg_skel-1.0.0/pcg_skel/pcg_skel.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 pcg_skel-1.0.0/pcg_skel/skel_utils.py
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 pcg_skel-1.0.0/pcg_skel/utils.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 pcg_skel-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 pcg_skel-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     9986 2020-02-02 00:00:00.000000 pcg_skel-1.0.0/README.md
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 pcg_skel-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    12758 2020-02-02 00:00:00.000000 pcg_skel-1.0.0/PKG-INFO
```

### Comparing `pcg_skel-0.3.5/LICENSE.txt` & `pcg_skel-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pcg_skel-0.3.5/PKG-INFO` & `pcg_skel-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,61 @@
-Metadata-Version: 2.1
-Name: pcg_skel
-Version: 0.3.5
+Metadata-Version: 2.3
+Name: pcg-skel
+Version: 1.0.0
 Summary: Skeletonization using the pychunkedgraph
-Home-page: https://github.com/AllenInstitute/pcg_skel
-Author: Casey Schneider-mizell
-Author-email: caseys@alleninstitute.org
-Description-Content-Type: text/markdown
+Project-URL: Repository, https://github.com/AllenInstitute/pcg_skel
+Author-email: Casey Schneider-mizell <caseys@alleninstitute.org>
+Maintainer-email: Casey Schneider-mizell <caseys@alleninstitute.org>
+License: Allen Institute Software License - This software license is the 2-clause BSD
+        license plus a third clause that prohibits redistribution for commercial
+        purposes without further permission.
+         
+        Copyright 2021. Allen Institute. All rights reserved.
+         
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+         
+        1. Redistributions of source code must retain the above copyright notice,
+        this list of conditions and the following disclaimer.
+         
+        2. Redistributions in binary form must reproduce the above copyright notice,
+        this list of conditions and the following disclaimer in the documentation
+        and/or other materials provided with the distribution.
+         
+        3. Redistributions for commercial purposes are not permitted without the
+        Allen Institute's written permission.
+        For purposes of this license, commercial purposes is the incorporation of the
+        Allen Institute's software into anything for which you will charge fees or
+        other compensation. Contact terms@alleninstitute.org for commercial licensing
+        opportunities.
+         
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+        ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+        LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+        CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+        SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+        INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+        CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+        ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+        POSSIBILITY OF SUCH DAMAGE.
 License-File: LICENSE.txt
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: pandas
-Requires-Dist: trimesh
-Requires-Dist: meshparty>=1.12.0
+Requires-Python: >=3.9
 Requires-Dist: caveclient>=4.12.4
-Requires-Dist: fastremap
 Requires-Dist: cloud-volume>=3.6.0
-Requires-Dist: sqlitedict
+Requires-Dist: fastremap
+Requires-Dist: meshparty>=1.12.0
+Requires-Dist: numpy
 Requires-Dist: orjson
+Requires-Dist: pandas
+Requires-Dist: scipy
+Requires-Dist: sqlitedict
+Requires-Dist: trimesh
+Description-Content-Type: text/markdown
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7703278.svg)](https://doi.org/10.5281/zenodo.7703278)
 
 # pcg_skel
 
 Generate robust neuronal topology directly from PyChunkedGraph dynamic segmentations.
```

### Comparing `pcg_skel-0.3.5/README.md` & `pcg_skel-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pcg_skel-0.3.5/pcg_skel/chunk_cache.py` & `pcg_skel-1.0.0/pcg_skel/chunk_cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from sqlitedict import SqliteDict
-import orjson
 import numpy as np
+import orjson
+from sqlitedict import SqliteDict
 
 POSITION_ATTRIBUTE = "rep_coord_nm"
 
 
 def get_locs_remote(l2_ids, client):
     """Retrieve ids from the l2 cache service"""
     l2_info = client.l2cache.get_l2data(list(l2_ids), attributes=[POSITION_ATTRIBUTE])
@@ -61,8 +61,7 @@
     """
     ii = 0
     with SqliteDict(cache_file, encode=orjson.dumps, flag="c") as cache_dict:
         for k, v in zip(l2_ids, l2_locs):
             if not np.any(np.isnan(v)):
                 cache_dict[str(k)] = v.tolist()
         cache_dict.commit()
-    pass
```

### Comparing `pcg_skel-0.3.5/pcg_skel/chunk_tools.py` & `pcg_skel-1.0.0/pcg_skel/chunk_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import numpy as np
-from scipy import spatial
 import cloudvolume
-from . import utils, chunk_cache, skel_utils
-import multiwrapper.multiprocessing_utils as mu
 import fastremap
+import multiwrapper.multiprocessing_utils as mu
+import numpy as np
+from scipy import spatial
+
+from . import chunk_cache, utils
 
 UnshardedMeshSource = (
     cloudvolume.datasource.graphene.mesh.unsharded.GrapheneUnshardedMeshSource
 )
 ShardedMeshSource = (
     cloudvolume.datasource.graphene.mesh.sharded.GrapheneShardedMeshSource
 )
```

### Comparing `pcg_skel-0.3.5/pcg_skel/features.py` & `pcg_skel-1.0.0/pcg_skel/features.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,37 @@
-import pandas as pd
 import numpy as np
+import pandas as pd
+import caveclient
+import datetime
+from meshparty import meshwork
+from meshparty.meshwork.algorithms import split_axon_by_annotation, strahler_order
+
 from . import pcg_anno
-from meshparty.meshwork.algorithms import strahler_order, split_axon_by_annotation
 
 VOL_PROPERTIES = ["area_nm2", "size_nm3", "mean_dt_nm", "max_dt_nm"]
 
 
 def add_synapses(
-    nrn,
-    synapse_table,
-    l2dict_mesh,
-    client,
-    root_id=None,
-    pre=False,
-    post=False,
-    remove_self_synapse=True,
-    timestamp=None,
-    live_query=False,
-    metadata=False,
-):
-    """Add synapses based on l2ids
+    nrn: meshwork.Meshwork,
+    synapse_table: str,
+    l2dict_mesh: dict,
+    client: caveclient.CAVEclient,
+    root_id: int = None,
+    pre: bool = False,
+    post: bool = False,
+    remove_self_synapse: bool = True,
+    timestamp: datetime.datetime = None,
+    live_query: bool = False,
+    metadata: bool = False,
+    synapse_partners: bool = False,
+    synapse_point_resolution: list[float] = None,
+    synapse_representative_point_pre: str = "ctr_pt_position",
+    synapse_representative_point_post: str = "ctr_pt_position",
+) -> None:
+    """Add synapses to a meshwork object based on l2ids
 
     Parameters
     ----------
     nrn : meshparty.meshwork.Meshwork
         Meshwork object
     synapse_table : str
         Annotation table to use for synapses
@@ -39,14 +47,17 @@
         If True, add postsynaptic synapses (i.e. inputs), by default False
     remove_self_synapse : bool, optional
         If True, omit synapses where the pre and post root ids are the same, by default True
     timestamp : datetime.datetime, optional
         Datetime to use for root id lookups if not using a materialized version, by default None
     live_query : bool, optional
         If True, use a timestamp to look up root ids, by default False
+    synapse_partners : bool, optional
+        If True, returns the root id of synapses partners in the dataframe.
+        By default, this is False because partner root ids change with editing and are not specified by this cell's data alone.
     """
     if root_id is None:
         root_id - nrn.seg_id
 
     pre_syn_df, post_syn_df = pcg_anno.get_level2_synapses(
         root_id,
         l2dict_mesh,
@@ -54,41 +65,44 @@
         synapse_table,
         remove_self=remove_self_synapse,
         pre=pre,
         post=post,
         live_query=live_query,
         timestamp=timestamp,
         metadata=metadata,
+        synapse_point_resolution=synapse_point_resolution,
     )
 
     if pre_syn_df is not None:
+        if not synapse_partners:
+            pre_syn_df = pre_syn_df.drop(columns=["post_pt_root_id"])
         nrn.anno.add_annotations(
             "pre_syn",
             pre_syn_df,
             index_column="pre_pt_mesh_ind",
-            point_column="ctr_pt_position",
-            voxel_resolution=pre_syn_df.attrs.get('dataframe_resolution'),
+            point_column=synapse_representative_point_pre,
+            voxel_resolution=pre_syn_df.attrs.get("dataframe_resolution"),
         )
     if post_syn_df is not None:
+        if not synapse_partners:
+            post_syn_df = post_syn_df.drop(columns=["pre_pt_root_id"])
         nrn.anno.add_annotations(
             "post_syn",
             post_syn_df,
             index_column="post_pt_mesh_ind",
-            point_column="ctr_pt_position",
-            voxel_resolution=post_syn_df.attrs.get('dataframe_resolution'),
+            point_column=synapse_representative_point_post,
+            voxel_resolution=post_syn_df.attrs.get("dataframe_resolution"),
         )
 
-    return
-
 
 def add_lvl2_ids(
-    nrn,
-    l2dict_mesh,
-    property_name="lvl2_ids",
-):
+    nrn: meshwork.Meshwork,
+    l2dict_mesh: dict,
+    property_name: str = "lvl2_ids",
+) -> None:
     """Add meshwork annotation table associating level 2 ids with vertex ids.
 
     Parameters
     ----------
     nrn : meshparty.meshwork.Meshwork
         Meshwork object
     l2dict_mesh : dict
@@ -96,25 +110,24 @@
     property_name : str, optional
         Name of the annotation table, by default "lvl2_ids"
     """
     lvl2_df = pd.DataFrame(
         {"lvl2_id": list(l2dict_mesh.keys()), "mesh_ind": list(l2dict_mesh.values())}
     )
     nrn.anno.add_annotations(property_name, lvl2_df, index_column="mesh_ind")
-    return
 
 
 def add_volumetric_properties(
-    nrn,
-    client,
-    attributes=VOL_PROPERTIES,
-    l2id_anno_name="lvl2_ids",
-    l2id_col_name="lvl2_id",
-    property_name="vol_prop",
-):
+    nrn: meshwork.Meshwork,
+    client: caveclient.CAVEclient,
+    attributes: list[str] = VOL_PROPERTIES,
+    l2id_anno_name: str = "lvl2_ids",
+    l2id_col_name: str = "lvl2_id",
+    property_name: str = "vol_prop",
+) -> None:
     """Add L2 Cache properties as an annotation property table.
 
     Parameters
     ----------
     nrn : meshparty.meshwork.Meshwork
         Meshwork object
     client : caveclient.CAVEclient
@@ -138,30 +151,28 @@
         property_name,
         data=l2_df.merge(dat_df, left_on=l2id_col_name, right_index=True).drop(
             columns=[l2id_col_name]
         ),
         index_column="mesh_ind",
     )
 
-    return
-
 
 def add_segment_properties(
-    nrn,
-    segment_property_name="segment_properties",
-    effective_radius=True,
-    area_factor=True,
-    strahler=True,
-    strahler_by_compartment=False,
-    volume_property_name="vol_prop",
-    volume_col_name="size_nm3",
-    area_col_name="area_nm2",
-    root_as_sphere=True,
-    comp_mask="is_axon",
-):
+    nrn: meshwork.Meshwork,
+    segment_property_name: str = "segment_properties",
+    effective_radius: bool = True,
+    area_factor: bool = True,
+    strahler: bool = True,
+    strahler_by_compartment: bool = False,
+    volume_property_name: str = "vol_prop",
+    volume_col_name: str = "size_nm3",
+    area_col_name: str = "area_nm2",
+    root_as_sphere: bool = True,
+    comp_mask: str = "is_axon",
+) -> None:
     """Use volumetric and topological properties to add descriptive properties for each skeleton vertex.
     Note that properties are estimated per segment, the unbranched region between branch points and/or endpoints.
 
     Parameters
     ----------
     nrn : meshparty.meshwork.Meshwork
         Meshwork object
@@ -263,35 +274,34 @@
         on="seg_num",
     )
     nrn.anno.add_annotations(
         segment_property_name,
         data=base_df,
         index_column="mesh_ind",
     )
-    return
 
 
 def add_is_axon_annotation(
-    nrn,
-    pre_anno,
-    post_anno,
-    annotation_name="is_axon",
-    threshold_quality=0.5,
-    extend_to_segment=True,
-    n_times=1,
-):
+    nrn: meshwork.Meshwork,
+    pre_anno: str,
+    post_anno: str,
+    annotation_name: str = "is_axon",
+    threshold_quality: float = 0.5,
+    extend_to_segment: bool = True,
+    n_times: int = 1,
+) -> None:
     """Add an annotation property table specifying which vertices belong to the axon, based on synaptic input and output locations
-    (see synapse flow centrality in "Quantitative neuroanatomy for connectomics in Drosophila", Schneider-Mizell et al. 2016)
+    For the synapse flow centrality algorithm, see "Quantitative neuroanatomy for connectomics in Drosophila", Schneider-Mizell et al. eLife 2016.
 
     Parameters
     ----------
     nrn : meshparty.meshwork.Meshwork
         Meshwork object
     pre_anno : str
-        Annotation property table name for presynaptic sites (outputs).  
+        Annotation property table name for presynaptic sites (outputs).
     post_anno : str
         Annotation property table name for postsyanptic sites (inputs).
     annotation_name : str, optional
         Name of the new table specifying axon indices, by default "is_axon"
     threshold_quality : float, optional
         Value between 0 and 1 setting the lower limit on input/output segregation quality, by default 0.5. If the segregatation quality is lower than this,
         a table is added but no vertices will be in the table.
@@ -310,17 +320,16 @@
         n_times=n_times,
     )
     if sq < threshold_quality:
         nrn.anno.add_annotations(annotation_name, [], mask=True)
         raise Warning("Split quality below threshold, no axon mesh vertices added!")
     else:
         nrn.anno.add_annotations(annotation_name, is_axon, mask=True)
-    return
 
 
 def l2dict_from_anno(
-    nrn,
-    table_name="lvl2_ids",
-    l2id_col="lvl2_id",
-    mesh_ind_col="mesh_ind",
-):
-    return nrn.anno[table_name].df.set_index(l2id_col)[mesh_ind_col].to_dict()
+    nrn: meshwork.Meshwork,
+    table_name: str = "lvl2_ids",
+    l2id_col: str = "lvl2_id",
+    mesh_ind_col: str = "mesh_ind",
+) -> dict:
+    return nrn.anno[table_name].df.set_index(l2id_col)[mesh_ind_col].to_dict()
```

### Comparing `pcg_skel-0.3.5/pcg_skel/nocache.py` & `pcg_skel-1.0.0/pcg_skel/nocache.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 DEFAULT_VOXEL_RESOLUTION = [4, 4, 40]
 DEFAULT_COLLAPSE_RADIUS = 7500.0
 DEFAULT_INVALIDATION_D = 7500
 
 skeleton_type = "pcg_skel"
 
+
 def chunk_index_mesh(
     root_id,
     client=None,
     datastack_name=None,
     cv=None,
     return_l2dict=False,
 ):
@@ -488,16 +489,14 @@
         output.append(missing_ids)
     if len(output) == 1:
         return output[0]
     else:
         return tuple(output)
 
 
-
-
 def pcg_meshwork(
     root_id,
     datastack_name=None,
     client=None,
     cv=None,
     refine="all",
     root_point=None,
@@ -632,66 +631,7 @@
 
     features.add_lvl2_ids(nrn, l2dict_mesh)
 
     if refine != "chunk":
         chunk_tools.adjust_meshwork(nrn, cv)
 
     return nrn
-
-
-
-
-def collapse_pcg_skeleton(soma_pt, sk, soma_r):
-    """Use soma point vertex and collapse soma as sphere
-    Parameters
-    ----------
-    soma_pt : array
-        3-element location of soma center (in nm)
-    sk: skeleton.Skeleton
-        Coarse skeleton
-    soma_r : float
-        Soma collapse radius (in nm)
-    Returns
-    -------
-    skeleton
-        New skeleton with updated properties
-    """
-    soma_verts, _ = skeletonize.soma_via_sphere(soma_pt, sk.vertices, sk.edges, soma_r)
-    min_soma_vert = np.argmin(np.linalg.norm(sk.vertices[soma_verts] - soma_pt, axis=1))
-    root_vert = soma_verts[min_soma_vert]
-
-    (
-        new_v,
-        new_e,
-        new_skel_map,
-        vert_filter,
-        root_ind,
-    ) = skeletonize.collapse_soma_skeleton(
-        soma_verts[soma_verts != root_vert],
-        soma_pt,
-        sk.vertices,
-        sk.edges,
-        sk.mesh_to_skel_map,
-        collapse_index=root_vert,
-        return_soma_ind=True,
-        return_filter=True,
-    )
-
-    new_mesh_index = sk.mesh_index[vert_filter]
-    new_skeleton = skeleton.Skeleton(
-        new_v,
-        new_e,
-        root=root_ind,
-        mesh_to_skel_map=new_skel_map,
-        mesh_index=new_mesh_index,
-        remove_zero_length_edges=False,
-        meta=sk.meta,
-    )
-
-    new_skeleton.meta.soma_pt_x = soma_pt[0]
-    new_skeleton.meta.soma_pt_y = soma_pt[1]
-    new_skeleton.meta.soma_pt_z = soma_pt[2]
-    new_skeleton.meta.soma_radius = soma_r
-    new_skeleton.meta.collapse_soma = True
-    new_skeleton.meta.collapse_function = "sphere"
-
-    return new_skeleton
```

### Comparing `pcg_skel-0.3.5/pcg_skel/pcg_anno.py` & `pcg_skel-1.0.0/pcg_skel/pcg_anno.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,25 @@
+from __future__ import annotations
 import datetime
 from caveclient.frameworkclient import CAVEclientFull
-import warnings
-
-try:
-    from annotationframeworkclient.frameworkclient import FrameworkClientFull
-
-    check_afc = True
-except:
-    FrameworkClientFull = type(None)
-    check_afc = False
+from typing import Union, Optional
+import pandas as pd
+from typing import Optional, Dict, Any, Tuple, Union, List
 
 
 def annotation_to_level2_id(
-    df,
-    client,
-    bound_pt_columns="pt",
-    l2_suffix="_level2_id",
-    sv_columns=None,
-    l2_columns=None,
-    inplace=False,
-    timestamp=None,
-):
+    df: pd.DataFrame,
+    client: CAVEclientFull,
+    bound_pt_columns: str = "pt",
+    l2_suffix: str = "_level2_id",
+    sv_columns: Optional[Union[str, list[str]]] = None,
+    l2_columns: Optional[Union[str, list[str]]] = None,
+    inplace: bool = False,
+    timestamp: Optional[datetime.datetime] = None,
+) -> pd.DataFrame:
     """Add or more level2_id columns to a dataframe based on supervoxel columns
 
     Parameters
     ----------
     df : pandas.DataFrame
         DataFrame with one or more supervoxel columns
     client : CAVEclient or ChunkedgraphClient
@@ -42,16 +37,16 @@
         If True, change the dataframe in place, by default False
     timestamp : datetime or None, optional
         Timestamp to lookup the mapping. If None, uses the materialization version timestamp.
         Default is None.
 
     Returns
     -------
-    [type]
-        [description]
+    pd.DataFrame
+        DataFrame with level 2 id columns added
     """
     if isinstance(bound_pt_columns, str):
         bound_pt_columns = [bound_pt_columns]
     if sv_columns is None:
         sv_columns = [f"{c}_supervoxel_id" for c in bound_pt_columns]
         if l2_columns is None:
             l2_columns = [f"{c}{l2_suffix}" for c in bound_pt_columns]
@@ -59,21 +54,14 @@
         l2_columns = [f"{c}{l2_suffix}" for c in sv_columns]
 
     if timestamp is None:
         timestamp = client.materialize.get_timestamp()
 
     if isinstance(client, CAVEclientFull):
         pcg_client = client.chunkedgraph
-    elif check_afc and isinstance(client, FrameworkClientFull):
-        warnings.warn(
-            DeprecationWarning(
-                "annotationframeworkclient is depricated. Please switch to using caveclient."
-            )
-        )
-        pcg_client = client.chunkedgraph
     else:
         pcg_client = client
 
     if not inplace:
         df = df.copy()
 
     for col, l2_col in zip(sv_columns, l2_columns):
@@ -83,20 +71,20 @@
             timestamp=timestamp,
         )
         df[l2_col] = level2_ids
     return df
 
 
 def annotation_to_mesh_index(
-    df,
-    l2dict,
-    level2_id_col="pt_level2_id",
-    mesh_index_col="pt_mesh_ind",
-    inplace=False,
-):
+    df: pd.DataFrame,
+    l2dict: dict,
+    level2_id_col: Union[str, list[str]] = "pt_level2_id",
+    mesh_index_col: str = "pt_mesh_ind",
+    inplace: bool = False,
+) -> pd.DataFrame:
     """Map level2 ids to mesh indices.
 
     Parameters
     ----------
     df : pandas.DataFrame
         DataFrame with at least one level 2 id column
     l2dict : dict
@@ -121,41 +109,132 @@
         mesh_index_col = [mesh_index_col]
 
     for l2col, mind_col in zip(level2_id_col, mesh_index_col):
         df[mind_col] = df[l2col].apply(lambda x: l2dict[x])
     return df
 
 
+def get_level2_synapses(
+    root_id: int,
+    l2dict: Dict[Any, Any],
+    client: CAVEclientFull,
+    synapse_table: str,
+    remove_self: bool = True,
+    pre: bool = True,
+    post: bool = True,
+    live_query: bool = False,
+    timestamp: Optional[datetime.datetime] = None,
+    metadata: bool = False,
+    synapse_point_resolution: Optional[List[float]] = None,
+) -> Tuple[Optional[pd.DataFrame], Optional[pd.DataFrame]]:
+    """Retrieve level 2 synapses for a given root ID.
+
+    Parameters
+    ----------
+    root_id : int
+        The root ID for which to retrieve synapses.
+    l2dict : dict
+        Dict of level2 id to mesh index mappings
+    client : object
+        The client object used for querying the synapse data.
+    synapse_table : str
+        The name of the synapse table to query.
+    remove_self : bool, optional
+        Whether to remove self-synapses. Defaults to True.
+    pre : bool, optional
+        Whether to retrieve pre-synapses. Defaults to True.
+    post : bool, optional
+        Whether to retrieve post-synapses. Defaults to True.
+    live_query : bool, optional
+        Whether to perform a live query. Defaults to False.
+    timestamp : datetime, optional
+        The timestamp for the live query. Defaults to None.
+    metadata : bool, optional
+        Whether to include metadata in the query results. Defaults to False.
+    synapse_point_resolution : list, optional
+        The resolution of the synapse points. Defaults to None.
+
+    Returns
+    -------
+    pre_syn_df : DataFrame or None
+        The DataFrame containing pre-synapse data, or None if pre is False.
+    post_syn_df : DataFrame or None
+        The DataFrame containing post-synapse data, or None if post is False.
+    """
+    live_query = timestamp is not None
+
+    if timestamp is None:
+        timestamp = datetime.datetime.utcnow()
+    if pre is True:
+        pre_syn_df = _mapped_synapses(
+            root_id,
+            client,
+            l2dict,
+            "pre",
+            synapse_table,
+            remove_self=remove_self,
+            live_query=live_query,
+            timestamp=timestamp,
+            metadata=metadata,
+            synapse_point_resolution=synapse_point_resolution,
+        )
+    else:
+        pre_syn_df = None
+
+    if post is True:
+        post_syn_df = _mapped_synapses(
+            root_id,
+            client,
+            l2dict,
+            "post",
+            synapse_table,
+            remove_self=remove_self,
+            live_query=live_query,
+            timestamp=timestamp,
+            metadata=metadata,
+            synapse_point_resolution=synapse_point_resolution,
+        )
+    else:
+        post_syn_df = None
+
+    return pre_syn_df, post_syn_df
+
+
 def _mapped_synapses(
     root_id,
     client,
     l2dict,
     side,
     synapse_table,
     remove_self,
     live_query,
     timestamp,
     metadata,
     remove_crud=True,
+    synapse_point_resolution=None,
 ):
     if live_query:
         syn_df = client.materialize.live_query(
             synapse_table,
             filter_equal_dict={f"{side}_pt_root_id": root_id},
             timestamp=timestamp,
-            metadata=metadata
+            metadata=metadata,
+            desired_resolution=synapse_point_resolution,
         )
     else:
         syn_df = client.materialize.query_table(
             synapse_table,
             filter_equal_dict={f"{side}_pt_root_id": root_id},
             metadata=metadata,
+            desired_resolution=synapse_point_resolution,
         )
     if remove_crud:
-        syn_df.drop(columns=['created', 'superceded_id', 'valid'], inplace=True, errors='ignore')
+        syn_df.drop(
+            columns=["created", "superceded_id", "valid"], inplace=True, errors="ignore"
+        )
 
     if remove_self:
         syn_df = syn_df.query("pre_pt_root_id != post_pt_root_id").reset_index(
             drop=True
         )
     syn_df = annotation_to_level2_id(
         syn_df,
@@ -168,56 +247,7 @@
         syn_df,
         l2dict,
         level2_id_col=f"{side}_pt_level2_id",
         mesh_index_col=f"{side}_pt_mesh_ind",
         inplace=True,
     )
     return syn_df
-
-
-def get_level2_synapses(
-    root_id,
-    l2dict,
-    client,
-    synapse_table,
-    remove_self=True,
-    pre=True,
-    post=True,
-    live_query=False,
-    timestamp=None,
-    metadata=False,
-):
-    live_query = timestamp is not None
-
-    if timestamp is None:
-        timestamp = datetime.datetime.utcnow()
-    if pre is True:
-        pre_syn_df = _mapped_synapses(
-            root_id,
-            client,
-            l2dict,
-            "pre",
-            synapse_table,
-            remove_self=remove_self,
-            live_query=live_query,
-            timestamp=timestamp,
-            metadata=metadata,
-        )
-    else:
-        pre_syn_df = None
-
-    if post is True:
-        post_syn_df = _mapped_synapses(
-            root_id,
-            client,
-            l2dict,
-            "post",
-            synapse_table,
-            remove_self=remove_self,
-            live_query=live_query,
-            timestamp=timestamp,
-            metadata=metadata,
-        )
-    else:
-        post_syn_df = None
-
-    return pre_syn_df, post_syn_df
```

### Comparing `pcg_skel-0.3.5/pcg_skel/pcg_skel.py` & `pcg_skel-1.0.0/pcg_skel/pcg_skel.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,64 @@
+from __future__ import annotations
+from . import chunk_tools, features
+from . import skel_utils as sk_utils
+
+import cloudvolume
+import warnings
 import numpy as np
+
 from caveclient import CAVEclient
-from meshparty import skeleton, skeletonize, trimesh_io, meshwork
+from meshparty import meshwork, skeletonize, trimesh_io
+from typing import Union, Optional
 
-from . import chunk_tools, features
-from . import skel_utils as sk_utils
-from . import utils
+Numeric = Union[int, float, np.number]
 
 DEFAULT_VOXEL_RESOLUTION = [4, 4, 40]
 DEFAULT_COLLAPSE_RADIUS = 7500.0
 DEFAULT_INVALIDATION_D = 7500
 
 skeleton_type = "pcg_skel"
 
-def coord_space_mesh(
-    root_id,
-    client,
-    cv=None,
-    return_l2dict=False,
-    nan_rounds=10,
-    require_complete=False,
+
+def pcg_graph(
+    root_id: int,
+    client: CAVEclient.frameworkclient.CAVEclientFull,
+    cv: cloudvolume.CloudVolume = None,
+    return_l2dict: bool = False,
+    nan_rounds: int = 10,
+    require_complete: bool = False,
 ):
     """Compute the level 2 spatial graph (or mesh) of a given root id using the l2cache.
 
+    Some text for you and me.
+
     Parameters
     ----------
     root_id : int
         Root id of a segment
     client : CAVEclient.caveclient
         Initialized CAVEclient for the dataset.
-    cv : cloudvolume.CloudVolume, optional
+    cv : cloudvolume.CloudVolume
         Initialized CloudVolume object for the dataset. This does not replace the caveclient, but
-        a pre-initizialized cloudvolume can save some time during batch processing. By default None. 
-    return_l2dict : bool, optional
-        If True, returns the mappings between l2 ids and vertices, by default False
-    nan_rounds : int, optional
-        If vertices are missing (or not computed), this sets the number of iterations for smoothing over them. By default 10
-    require_complete : bool, optional
-        If True, raise an Exception if any vertices are missing from the cache, by default False
+        a pre-initizialized cloudvolume can save some time during batch processing.
+    return_l2dict : bool
+        If True, returns the mappings between l2 ids and vertices.
+    nan_rounds : int
+        If vertices are missing (or not computed), this sets the number of iterations for smoothing over them.
+    require_complete : bool
+        If True, raise an Exception if any vertices are missing from the cache.
+
 
     Returns
     -------
     mesh : meshparty.trimesh_io.Mesh
         Object with a vertex for every level 2 id and edges between all connected level 2 chunks.
-    l2dict : dict (optional)
+    l2dict : dict, optional
         Dictionary with keys as level 2 ids and values as mesh vertex index. Optional, only returned if `return_l2dict` is True.
-    l2dict_reverse : dict (optional)
+    l2dict_reverse : dict, optional
         Dictionary with keys as mesh vertex indices and values as level 2 id. Optional, only returned if `return_l2dict` is True.
     """
     if cv is None:
         cv = client.info.segmentation_cloudvolume(progress=False)
 
     lvl2_eg = client.chunkedgraph.level2_chunk_graph(root_id)
     eg, l2dict_mesh, l2dict_r_mesh, x_ch = chunk_tools.build_spatial_graph(
@@ -68,94 +78,156 @@
 
     if return_l2dict:
         return mesh_loc, l2dict_mesh, l2dict_r_mesh
     else:
         return mesh_loc
 
 
-def coord_space_skeleton(
-    root_id,
-    client,
-    datastack_name=None,
-    cv=None,
-    invalidation_d=10_000,
-    return_mesh=False,
-    return_l2dict=False,
-    return_l2dict_mesh=False,
-    root_point=None,
-    root_point_resolution=None,
-    collapse_soma=False,
-    collapse_radius=7500,
-    nan_rounds=10,
-    require_complete=False,
+def pcg_skeleton_direct(
+    vertices,
+    edges,
+    invalidation_d: Numeric = DEFAULT_INVALIDATION_D,
+    root_point: list = None,
+    collapse_soma: bool = False,
+    collapse_radius: Numeric = DEFAULT_COLLAPSE_RADIUS,
+    root_id: Optional[int] = None,
+):
+    """
+    Produce a skeleton from an already-computed l2graph.
+    This is effectively a wrapper for meshparty skeletonize with a consistent set of parameters and format.
+
+    Parameters
+    ----------
+    vertices : np.array
+        Array of vertices for the mesh graph.
+    edges : np.array
+        Array of edges for the mesh graph.
+    invalidation_d : int, optional
+        Distance (in nanometers) for TEASAR skeleton invalidation.
+    root_point : np.array, optional
+        3-element list or array with the x,y,z location of the root point in same units as vertices.
+        If None, the most distant tip is set to root.
+    collapse_soma : bool, optional
+        If True, collapse nearby vertices into the root point.
+    collapse_radius : int, optional
+        Distance (in nanometers) for soma collapse.
+    root_id : int, optional
+        Root id of the segment, used in metadata. Optional, by default None.
+
+    Returns
+    -------
+    sk : meshparty.skeleton.Skeleton
+        Skeleton for the l2graph.
+    """
+
+    l2graph = trimesh_io.Mesh(
+        vertices=vertices,
+        faces=[[0, 0, 0]],  # Some functions fail if no faces are set.
+        link_edges=edges,
+    )
+
+    sk = skeletonize.skeletonize_mesh(
+        l2graph,
+        invalidation_d=invalidation_d,
+        soma_pt=root_point,
+        collapse_soma=collapse_soma,
+        soma_radius=collapse_radius,
+        compute_radius=False,
+        cc_vertex_thresh=0,
+        remove_zero_length_edges=True,
+        meta={
+            "root_id": root_id,
+            "skeleton_type": skeleton_type,
+            "meta": {"space": "l2cache", "datastack": None},
+        },
+    )
+    return sk
+
+
+def pcg_skeleton(
+    root_id: int,
+    client: CAVEclient.frameworkclient.CAVEclientFull,
+    datastack_name: str = None,
+    cv: cloudvolume.CloudVolume = None,
+    invalidation_d: Numeric = 7500,
+    return_mesh: bool = False,
+    return_l2dict: bool = False,
+    return_l2dict_mesh: bool = False,
+    root_point: list = None,
+    root_point_resolution: list = None,
+    collapse_soma: bool = False,
+    collapse_radius: Numeric = 7500,
+    nan_rounds: int = 10,
+    require_complete: bool = False,
 ):
     """Produce a skeleton from the level 2 graph.
     Parameters
     ----------
     root_id : int
         Root id of a segment
-    client : CAVEclient.caveclient
+    client : CAVEclient.caveclient.CAVEclientFull
         Initialized CAVEclient for the dataset.
     datastack_name : string, optional
-        If client is None, initializes a CAVEclient at this datastack, by default None.
+        If client is None, initializes a CAVEclient at this datastack.
     cv : cloudvolume.CloudVolume, optional
         Initialized CloudVolume object for the dataset. This does not replace the caveclient, but
-        a pre-initizialized cloudvolume can save some time during batch processing. By default None. 
+        a pre-initizialized cloudvolume can save some time during batch processing.
     invalidation_d : int, optional
-        Distance (in nanometers) for TEASAR skeleton invalidation, by default 10_000.
+        Distance (in nanometers) for TEASAR skeleton invalidation.
     return_mesh : bool, optional
-        If True, returns the mesh graph as well as the skeleton, by default False
+        If True, returns the mesh graph as well as the skeleton.
     return_l2dict : bool, optional
-        If True, returns the mappings between l2 ids and skeleton vertices, by default False
+        If True, returns the mappings between l2 ids and skeleton vertices.
     return_l2dict_mesh : bool, optional
-        If True, returns mappings between l2 ids and mesh graph vertices, by default False
-    root_point : list-like, optional
-        3-element list or array with the x,y,z location of the root point. Optional, by default None.
+        If True, returns mappings between l2 ids and mesh graph vertices.
+    root_point : npt.ArrayLike, optional
+        3-element list or array with the x,y,z location of the root point.
         If None, the most distant tip is set to root.
-    root_point_resolution : list-like, optional
-        3-element list or array with the x,y,z resolution of the root point, in nanometers per voxel dimension, by default None.
+    root_point_resolution : npt.ArrayLike, optional
+        3-element list or array with the x,y,z resolution of the root point, in nanometers per voxel dimension.
     collapse_soma : bool, optional
-        If True, collapse nearby vertices into the root point, by default False.
+        If True, collapse nearby vertices into the root point.
     collapse_radius : int, optional
-        Distance (in nanometers) for soma collapse, by default 7500.
+        Distance (in nanometers) for soma collapse.
     nan_rounds : int, optional
-        If vertices are missing (or not computed), this sets the number of iterations for smoothing over them. By default 10
+        If vertices are missing (or not computed), this sets the number of iterations for smoothing over them.
     require_complete : bool, optional
-        If True, raise an Exception if any vertices are missing from the cache, by default False
+        If True, raise an Exception if any vertices are missing from the cache.
 
     Returns
     -------
     sk : meshparty.skeleton.Skeleton
         Skeleton for the root id
-    mesh : meshparty.trimesh_io.Mesh (optional)
+    mesh : meshparty.trimesh_io.Mesh, optional
         Mesh graph that the skeleton is based on, only returned if return_mesh is True.
-    (l2dict_skel, l2dict_reverse): tuple of dicts (optional)
+    (l2dict_skel, l2dict_reverse): (dict, dict), optional
         Dictionaries mapping l2 ids to skeleton vertices and skeleton vertices to l2 ids, respectively. Only returned if return_l2dict is True.
-    (l2dict_mesh, l2dict_mesh): tuple of dicts (optional)
+    (l2dict_mesh, l2dict_mesh): (dict, dict), optional
         Dictionaries mapping l2 ids to mesh graph vertices and mesh_graph vertices to l2 ids, respectively. Only returned if return_l2dict is True.
     """
     if client is None:
         client = CAVEclient(datastack_name)
     if cv is None:
         cv = client.info.segmentation_cloudvolume(progress=False)
 
     if root_point_resolution is None:
         root_point_resolution = cv.mip_resolution(0)
     if root_point is not None:
         root_point = np.array(root_point) * root_point_resolution
 
-    mesh, l2dict_mesh, l2dict_r_mesh = coord_space_mesh(
+    mesh, l2dict_mesh, l2dict_r_mesh = pcg_graph(
         root_id,
         client=client,
         return_l2dict=True,
         nan_rounds=nan_rounds,
         require_complete=require_complete,
     )
 
     metameta = {"space": "l2cache", "datastack": client.datastack_name}
+
     sk = skeletonize.skeletonize_mesh(
         mesh,
         invalidation_d=invalidation_d,
         soma_pt=root_point,
         collapse_soma=collapse_soma,
         soma_radius=collapse_radius,
         compute_radius=False,
@@ -179,15 +251,15 @@
         out_list.append((l2dict_mesh, l2dict_r_mesh))
     if len(out_list) == 1:
         return out_list[0]
     else:
         return tuple(out_list)
 
 
-def coord_space_meshwork(
+def pcg_meshwork(
     root_id,
     datastack_name=None,
     client=None,
     cv=None,
     root_point=None,
     root_point_resolution=None,
     collapse_soma=False,
@@ -196,15 +268,19 @@
     synapse_table=None,
     remove_self_synapse=True,
     live_query=False,
     timestamp=None,
     invalidation_d=DEFAULT_INVALIDATION_D,
     require_complete=False,
     metadata=False,
-):
+    synapse_partners=False,
+    synapse_point_resolution=[1, 1, 1],
+    synapse_representative_point_pre="ctr_pt_position",
+    synapse_representative_point_post="ctr_pt_position",
+) -> meshwork.Meshwork:
     """Generate a meshwork file based on the level 2 graph.
 
     Parameters
     ----------
     root_id : int
         Root id of an object in the pychunkedgraph.
     datastack_name : str or None, optional
@@ -219,42 +295,54 @@
     root_point_resolution : array-like, optional
         Resolution in euclidean space of the root_point, by default [4, 4, 40]
     collapse_soma : bool, optional,
         If True, collapses vertices within a given radius of the root point into the root vertex, typically to better
         represent primary neurite branches. Requires a specified root_point. Default if False.
     collapse_radius : float, optional
         Max distance in euclidean space for soma collapse. Default is 10,000 nm (10 microns).
-    synapses : 'pre', 'post', 'all', or None, optional
-        If not None, queries the synapse_table for presynaptic synapses (if 'pre'),  postsynaptic sites (if 'post'), or both (if 'all'). By default None
+    synapses : 'pre', 'post', 'all', True, or None, optional
+        If not None, queries the synapse_table for presynaptic synapses (if 'pre'),  postsynaptic sites (if 'post'), or both (if 'all' or True). By default None
     synapse_table : str, optional
         Name of the synapse table to query if synapses are requested, by default None
     remove_self_synapse : bool, optional
         If True, filters out synapses whose pre- and postsynaptic root ids are the same neuron, by default True
     live_query : bool, optional
         If True, expect a timestamp for querying at a give point in time. Otherwise, use the materializatio set by the client. Optional, by default False.
     timestamp = datetime.datetime, optional
-        If set, acts as the time at which all root ids and annotations are found at. 
+        If set, acts as the time at which all root ids and annotations are found at.
     invalidation_d : int, optional
         Invalidation radius in hops for the mesh skeletonization along the chunk adjacency graph, by default 3
     require_complete : bool, optional
         If True, raise an Exception if any vertices are missing from the cache, by default False
+    metadata : bool, optional
+        If True, adds metadata to the meshwork annotations. By default False.
+    synapse_partners : bool, optional
+        If True, includes the partner root id to the synapse annotation. By default False, because partner roots can change across time.
+    synapse_point_resolution : array-like, optional
+        Resolution in euclidean space of the synapse points, by default None. If None, the resolution will be the default of the synapse table.
+    synapse_representative_point_pre : str, optional
+        If set, uses the specified column in the synapse table for the pre-synaptic points. By default 'ctr_pt_position'.
+    synapse_representative_point_post : str, optional
+        If set, uses the specified column in the synapse table for the post-synaptic points. By default 'ctr_pt_position'.
 
     Returns
     -------
     meshparty.meshwork.Meshwork
         Meshwork object with skeleton based on the level 2 graph. See documentation for details.
     """
     if client is None:
         client = CAVEclient(datastack_name)
     if cv is None:
         cv = client.info.segmentation_cloudvolume(progress=True, parallel=1)
     if root_point_resolution is None:
         root_point_resolution = cv.mip_resolution(0)
+    if synapse_table is None:
+        synapse_table = client.materialize.synapse_table
 
-    sk, mesh, (l2dict_mesh, l2dict_mesh_r) = coord_space_skeleton(
+    sk, mesh, (l2dict_mesh, l2dict_mesh_r) = pcg_skeleton(
         root_id,
         client=client,
         cv=cv,
         root_point=root_point,
         root_point_resolution=root_point_resolution,
         collapse_soma=collapse_soma,
         collapse_radius=collapse_radius,
@@ -268,18 +356,18 @@
 
     pre, post = False, False
     if synapses is not None and synapse_table is not None:
         if synapses == "pre":
             pre, post = True, False
         elif synapses == "post":
             pre, post = False, True
-        elif synapses == "all":
+        elif synapses == "all" or synapses is True:
             pre, post = True, True
         else:
-            raise ValueError('Synapses must be one of "pre", "post", or "all".')
+            raise ValueError('Synapses must be one of "pre", "post", or "all" or True.')
 
         if not timestamp:
             timestamp = client.materialize.get_timestamp()
 
         features.add_synapses(
             nrn,
             synapse_table,
@@ -288,701 +376,237 @@
             root_id=root_id,
             pre=pre,
             post=post,
             remove_self_synapse=remove_self_synapse,
             timestamp=timestamp,
             live_query=live_query,
             metadata=metadata,
+            synapse_partners=synapse_partners,
+            synapse_point_resolution=synapse_point_resolution,
+            synapse_representative_point_pre=synapse_representative_point_pre,
+            synapse_representative_point_post=synapse_representative_point_post,
         )
 
     features.add_lvl2_ids(nrn, l2dict_mesh)
     return nrn
 
 
-
-def chunk_index_mesh(
-    root_id,
-    client=None,
-    datastack_name=None,
-    cv=None,
-    return_l2dict=False,
-):
-    """Download a mesh with chunk index vertices
-
-    Parameters
-    ----------
-    root_id : int
-        Root id to download.
-    client : CAVEclient, optional
-        Preset CAVEclient, by default None.
-    datastack_name : str or None, optional
-        Datastack to use to initialize a CAVEclient, by default None.
-    cv : cloudvolume.CloudVolume or None, optional
-        Cloudvolume instance, by default None.
-    return_l2dict : bool, optional
-        If True, returns both a l2id to vertex dict and the reverse, by default False.
-
-    Returns
-    -------
-    mesh : trimesh_io.Mesh
-        Chunk graph represented as a mesh, with vertices at chunk index locations and edges in the link_edges attribute.
-    l2dict_mesh : dict
-        l2 id to mesh vertex index dictionary. Only returned if return_l2dict is True.
-    l2dict_r_mesh : dict
-        Mesh vertex index to l2 id dictionary. Only returned if return_l2dict is True.
-    """
-    DeprecationWarning('This function does not use the L2cache natively and will be moved to pcg_skel.nocache in a future version.')
-
-    if client is None:
-        client = CAVEclient(datastack_name)
-    if cv is None:
-        cv = client.info.segmentation_cloudvolume(progress=False)
-
-    lvl2_eg = client.chunkedgraph.level2_chunk_graph(root_id)
-    eg, l2dict_mesh, l2dict_r_mesh, x_ch = chunk_tools.build_spatial_graph(lvl2_eg, cv)
-    mesh_chunk = trimesh_io.Mesh(
-        vertices=x_ch,
-        faces=[[0, 0, 0]],  # Some functions fail if no faces are set.
-        link_edges=eg,
-    )
-    if return_l2dict:
-        return mesh_chunk, l2dict_mesh, l2dict_r_mesh
-    else:
-        return mesh_chunk
-
-
-def chunk_index_skeleton(
+def coord_space_skeleton(
     root_id,
-    client=None,
+    client,
     datastack_name=None,
     cv=None,
-    root_point=None,
-    invalidation_d=3,
+    invalidation_d=10_000,
     return_mesh=False,
     return_l2dict=False,
-    return_mesh_l2dict=False,
+    return_l2dict_mesh=False,
+    root_point=None,
     root_point_resolution=None,
-    root_point_search_radius=300,
-    n_parallel=1,
+    collapse_soma=False,
+    collapse_radius=7500,
+    nan_rounds=10,
+    require_complete=False,
 ):
-    """Generate a basic skeleton with chunked-graph index vertices.
+    """Produce a skeleton from the level 2 graph.
+
+    **Deprecated: Please use pcg_skeleton instead.**
 
     Parameters
     ----------
-    root_id : np.uint64
-        Neuron root id
-    client : caveclient.CAVEclient, optional
-        CAVEclient for a datastack, by default None. If None, you must specify a datastack name.
-    datastack_name : str, optional
-        Datastack name to create a CAVEclient, by default None. Only used if client is None.
+    root_id : int
+        Root id of a segment
+    client : CAVEclient.caveclient
+        Initialized CAVEclient for the dataset.
+    datastack_name : string, optional
+        If client is None, initializes a CAVEclient at this datastack, by default None.
     cv : cloudvolume.CloudVolume, optional
-        CloudVolume associated with the object, by default None. If None, one is created based on the client info.
-    root_point : array, optional
-        Point in voxel space to set the root vertex. By default None, which makes a random tip root.
+        Initialized CloudVolume object for the dataset. This does not replace the caveclient, but
+        a pre-initizialized cloudvolume can save some time during batch processing. By default None.
     invalidation_d : int, optional
-        TEASAR invalidation radius in chunk space, by default 3
+        Distance (in nanometers) for TEASAR skeleton invalidation, by default 10_000.
     return_mesh : bool, optional
-        If True, returns the pre-skeletonization mesh with vertices in chunk index space, by default False
+        If True, returns the mesh graph as well as the skeleton, by default False
     return_l2dict : bool, optional
-        If True, returns the level 2 id to vertex index dict. By default True
-    n_parallel : int, optional
-        Sets number of parallel threads for cloudvolume, by default 1
+        If True, returns the mappings between l2 ids and skeleton vertices, by default False
+    return_l2dict_mesh : bool, optional
+        If True, returns mappings between l2 ids and mesh graph vertices, by default False
+    root_point : list-like, optional
+        3-element list or array with the x,y,z location of the root point. Optional, by default None.
+        If None, the most distant tip is set to root.
+    root_point_resolution : list-like, optional
+        3-element list or array with the x,y,z resolution of the root point, in nanometers per voxel dimension, by default None.
+    collapse_soma : bool, optional
+        If True, collapse nearby vertices into the root point, by default False.
+    collapse_radius : int, optional
+        Distance (in nanometers) for soma collapse, by default 7500.
+    nan_rounds : int, optional
+        If vertices are missing (or not computed), this sets the number of iterations for smoothing over them. By default 10
+    require_complete : bool, optional
+        If True, raise an Exception if any vertices are missing from the cache, by default False
 
     Returns
     -------
     sk : meshparty.skeleton.Skeleton
-        Skeleton object
-    mesh : meshparty.trimesh_io.Mesh
-        Mesh object, only if return_mesh is True
-    level2_dict : dict
-        Level 2 id to vertex map, only if return_l2dict is True.
+        Skeleton for the root id
+    mesh : meshparty.trimesh_io.Mesh (optional)
+        Mesh graph that the skeleton is based on, only returned if return_mesh is True.
+    (l2dict_skel, l2dict_reverse): tuple of dicts (optional)
+        Dictionaries mapping l2 ids to skeleton vertices and skeleton vertices to l2 ids, respectively. Only returned if return_l2dict is True.
+    (l2dict_mesh, l2dict_mesh): tuple of dicts (optional)
+        Dictionaries mapping l2 ids to mesh graph vertices and mesh_graph vertices to l2 ids, respectively. Only returned if return_l2dict is True.
     """
-    DeprecationWarning('This function does not use the L2cache natively and will be moved to pcg_skel.nocache in a future version.')
-
-    if client is None:
-        client = CAVEclient(datastack_name)
-    if n_parallel is None:
-        n_parallel = 1
-    if cv is None:
-        cv = client.info.segmentation_cloudvolume(progress=True, parallel=1)
-
-    if root_point_resolution is None:
-        root_point_resolution = cv.mip_resolution(0)
-
-    mesh_chunk, l2dict_mesh, l2dict_r_mesh = chunk_index_mesh(
-        root_id, client=client, cv=cv, return_l2dict=True
+    warnings.warn(
+        "The function `coord_space_skeleton` is deprecated and has been replaced with 'pcg_skeleton'",
+        DeprecationWarning,
     )
-
-    if root_point is not None:
-        lvl2_root_chid, lvl2_root_loc = chunk_tools.get_closest_lvl2_chunk(
-            root_point,
-            root_id,
-            client=client,
-            cv=None,
-            radius=root_point_search_radius,
-            voxel_resolution=root_point_resolution,
-            return_point=True,
-        )  # Need to have cv=None because of a cloudvolume inconsistency
-        root_mesh_index = l2dict_mesh[lvl2_root_chid]
-    else:
-        root_mesh_index = None
-
-    metameta = {"space": "chunk", "datastack": client.datastack_name}
-    sk_ch = skeletonize.skeletonize_mesh(
-        mesh_chunk,
-        invalidation_d=invalidation_d,
-        collapse_soma=False,
-        compute_radius=False,
-        cc_vertex_thresh=0,
-        root_index=root_mesh_index,
-        remove_zero_length_edges=False,
-        meta={
-            "root_id": root_id,
-            "skeleton_type": skeleton_type,
-            "meta": metameta,
-        },
-    )
-
-    l2dict, l2dict_r = sk_utils.filter_l2dict(sk_ch, l2dict_r_mesh)
-
-    out_list = [sk_ch]
-    if return_mesh:
-        out_list.append(mesh_chunk)
-    if return_l2dict:
-        out_list.append((l2dict, l2dict_r))
-    if return_mesh_l2dict:
-        out_list.append((l2dict_mesh, l2dict_r_mesh))
-    if len(out_list) == 1:
-        return out_list[0]
-    else:
-        return tuple(out_list)
-
-
-def refine_chunk_index_skeleton(
-    sk_ch,
-    l2dict_reversed,
-    cv,
-    refine_inds="all",
-    scale_chunk_index=True,
-    root_location=None,
-    nan_rounds=20,
-    return_missing_ids=False,
-    segmentation_fallback=False,
-    fallback_mip=2,
-    cache=None,
-    save_to_cache=False,
-    client=None,
-    l2cache=False,
-):
-    """Refine skeletons in chunk index space to Euclidean space.
-
-    Parameters
-    ----------
-    sk_ch : meshparty.skeleton.Skeleton
-        Skeleton in chunk index space
-    l2dict_reversed : dict
-        Mapping between skeleton vertex index and level 2 id.
-    cv : cloudvolume.CloudVolume
-        Associated cloudvolume
-    refine_inds : str, None or list-like, optional
-        Skeleton indices to refine, 'all', or None. If 'all', does all skeleton indices.
-        If None, downloads no index but can use other options.
-        By default 'all'.
-    scale_chunk_index : bool, optional
-        If True, maps unrefined chunk index locations to the center of the chunk in
-        Euclidean space, by default True
-    root_location : list-like, optional
-        3-element euclidean space location to which to map the root vertex location, by default None
-    nan_rounds : int, optional
-        Number of passes to smooth over any missing values by averaging proximate vertex locations.
-        Only used if refine_inds is 'all'. Default is 20.
-    return_missing_ids : bool, optional
-        If True, returns ids of any missing level 2 meshes. Default is False
-    segmentation_fallback : bool, optional
-        If True, downloads the segmentation at mip level in fallback_mip to get a location. Very slow. Default is False.
-    fallback_mip : int, optional
-        The mip level used in segmentation fallback. Default is 2.
-    cache : str, optional
-        If set to 'service', uses the l2cache service if available available. Otherwise, a filename for a sqlite database storing locations associated with level 2 ids. Default is None.
-    save_to_cache : bool, optional
-        If using a sqlite database, setting this to True will add values to the cache as downloads occur.
-    client : CAVEclient, optional
-        If using the l2cache service, provides a client that can access it.
-    l2cache : bool, optional,
-        Set to True if using a l2cache to localize vertices. Same as setting cache to 'service'. Default is False.
-
-    Returns
-    -------
-    meshparty.skeleton.Skeleton
-        Skeleton with remapped vertex locations
-    """
-    if nan_rounds is None:
-        convert_missing = True
-    else:
-        convert_missing = False
-
-    if l2cache:
-        cache = "service"
-
-    refine_out = chunk_tools.refine_vertices(
-        sk_ch.vertices,
-        l2dict_reversed=l2dict_reversed,
+    return pcg_skeleton(
+        root_id,
+        client,
+        datastack_name=datastack_name,
         cv=cv,
-        refine_inds=refine_inds,
-        scale_chunk_index=scale_chunk_index,
-        convert_missing=convert_missing,
-        return_missing_ids=return_missing_ids,
-        segmentation_fallback=segmentation_fallback,
-        fallback_mip=fallback_mip,
-        cache=cache,
-        save_to_cache=save_to_cache,
-        client=client,
+        invalidation_d=invalidation_d,
+        return_mesh=return_mesh,
+        return_l2dict=return_l2dict,
+        return_l2dict_mesh=return_l2dict_mesh,
+        root_point=root_point,
+        root_point_resolution=root_point_resolution,
+        collapse_soma=collapse_soma,
+        collapse_radius=collapse_radius,
+        nan_rounds=nan_rounds,
+        require_complete=require_complete,
     )
-    if return_missing_ids:
-        new_verts, missing_ids = refine_out
-    else:
-        new_verts = refine_out
-
-    if root_location is not None:
-        new_verts[sk_ch.root] = root_location
 
-    l2_sk = skeleton.Skeleton(
-        vertices=new_verts,
-        edges=sk_ch.edges,
-        root=sk_ch.root,
-        remove_zero_length_edges=False,
-        mesh_index=sk_ch.mesh_index,
-        mesh_to_skel_map=sk_ch.mesh_to_skel_map,
-        meta=sk_ch.meta,
-    )
-    metameta = {
-        "space": "euclidean",
-    }
-    try:
-        l2_sk.meta.update_metameta(metameta)
-    except:
-        pass
 
-    if isinstance(refine_inds, str) and refine_inds == "all":
-        sk_utils.fix_nan_verts(l2_sk, num_rounds=nan_rounds)
-
-    if return_missing_ids:
-        return l2_sk, missing_ids
-    else:
-        return l2_sk
-
-
-def pcg_skeleton(
+def coord_space_mesh(
     root_id,
-    client=None,
-    datastack_name=None,
+    client,
     cv=None,
-    refine="all",
-    root_point=None,
-    root_point_resolution=None,
-    root_point_search_radius=300,
-    collapse_soma=False,
-    collapse_radius=10_000.0,
-    invalidation_d=3,
-    return_mesh=False,
     return_l2dict=False,
-    return_l2dict_mesh=False,
-    return_missing_ids=False,
-    nan_rounds=20,
-    segmentation_fallback=False,
-    fallback_mip=2,
-    cache=None,
-    save_to_cache=False,
-    n_parallel=1,
-    l2cache=False,
+    nan_rounds=10,
+    require_complete=False,
 ):
-    """Create a euclidean-space skeleton from the pychunkedgraph
+    """Compute the level 2 spatial graph (or mesh) of a given root id using the l2cache.
+    Deprecated: Use pcg_graph instead.
 
     Parameters
     ----------
-    root_id : uint64
-        Root id of the neuron to skeletonize
-    client : caveclient.CAVEclientFull or None, optional
-        Pre-specified cave client for the pcg. If this is not set, datastack_name must be provided. By default None
-    datastack_name : str or None, optional
-        If no client is specified, a CAVEclient is created with this datastack name, by default None
-    cv : cloudvolume.CloudVolume or None, optional
-        Prespecified cloudvolume instance. If None, uses the client info to make one, by default None
-    refine : 'all', 'ep', 'bp', 'epbp', 'bpep', or None, optional
-        Selects how to refine vertex locations by downloading mesh chunks. Unrefined vertices are placed in the
-        center of their chunk in euclidean space.
-        * 'all' refines all vertex locations. (Default)
-        * 'ep' refines end points only
-        * 'bp' refines branch points only
-        * 'bpep' or 'epbp' refines both branch and end points.
-        * None refines no points.
-        * 'chunk' Keeps things in chunk index space.
-    root_point : array-like or None, optional
-        3 element xyz location for the location to set the root in units set by root_point_resolution,
-        by default None. If None, a distal tip is selected.
-    root_point_resolution : array-like, optional
-        Resolution in euclidean space of the root_point, by default [4, 4, 40]
-    root_point_search_radius : int, optional
-        Distance in euclidean space to look for segmentation when finding the root vertex, by default 300
-    collapse_soma : bool, optional,
-        If True, collapses vertices within a given radius of the root point into the root vertex, typically to better
-        represent primary neurite branches. Requires a specified root_point. Default if False.
-    collapse_radius : float, optional
-        Max distance in euclidean space for soma collapse. Default is 10,000 nm (10 microns).
-    invalidation_d : int, optional
-        Invalidation radius in hops for the mesh skeletonization along the chunk adjacency graph, by default 3
-    return_mesh : bool, optional
-        If True, returns the mesh in chunk index space, by default False
+    root_id : int
+        Root id of a segment
+    client : CAVEclient.caveclient
+        Initialized CAVEclient for the dataset.
+    cv : cloudvolume.CloudVolume, optional
+        Initialized CloudVolume object for the dataset. This does not replace the caveclient, but
+        a pre-initizialized cloudvolume can save some time during batch processing. By default None.
     return_l2dict : bool, optional
-        If True, returns the tuple (l2dict, l2dict_r), by default False.
-        l2dict maps all neuron level2 ids to skeleton vertices. l2dict_r maps skeleton indices to their direct level 2 id.
-    return_l2dict_mesh : bool, optional
-        If True, returns the tuple (l2dict_mesh, l2dict_mesh_r), by default False.
-        l2dict_mesh maps neuron level 2 ids to mesh vertices, l2dict_r maps mesh indices to level 2 ids.
-    return_missing_ids : bool, optional
-        If True, returns level 2 ids that were missing in the chunkedgraph, by default False. This can be useful
-        for submitting remesh requests in case of errors.
+        If True, returns the mappings between l2 ids and vertices, by default False
     nan_rounds : int, optional
-        Maximum number of rounds of smoothing to eliminate missing vertex locations in the event of a
-        missing level 2 mesh, by default 20. This is only used when refine=='all'.
-    segmentation_fallback : bool, optional
-        If True, uses the segmentation in cases of missing level 2 meshes. This is slower but more robust.
-        Default is True.
-    cache : str or None, optional
-        If set to 'service', uses the online l2cache service (if available). Otherwise, this is the filename of a sqlite database with cached lookups for l2 ids. Optional, default is None.
-    n_parallel : int, optional
-        Number of parallel downloads passed to cloudvolume, by default 1
-    l2cache : bool, optional
-        Set to True if using the l2cache. Equivalent to cache='service'. Default is False.
+        If vertices are missing (or not computed), this sets the number of iterations for smoothing over them. By default 10
+    require_complete : bool, optional
+        If True, raise an Exception if any vertices are missing from the cache, by default False
 
     Returns
     -------
-    sk_l2 : meshparty.skeleton.Skeleton
-        Skeleton with vertices in euclidean space
-    mesh_l2 : meshparty.mesh.Mesh, optional
-        Mesh with vertices in chunk index space. Only if return_mesh is True.
-    (l2dict, l2dict_r) : (dict, dict), optional
-        Mappings between level 2 ids and skeleton indices. Only if return_l2dict is True.
-    (l2dict_mesh, l2dict_mesh_r) : (dict, dict), optional
-        Mappings between level 2 ids and mesh indices. Only if return_l2dict_mesh is True.
-    missing_ids : np.array, optional
-        List of level 2 ids with missing mesh fragments. Only if return_missing_ids is True.
+    mesh : meshparty.trimesh_io.Mesh
+        Object with a vertex for every level 2 id and edges between all connected level 2 chunks.
+    l2dict : dict (optional)
+        Dictionary with keys as level 2 ids and values as mesh vertex index. Optional, only returned if `return_l2dict` is True.
+    l2dict_reverse : dict (optional)
+        Dictionary with keys as mesh vertex indices and values as level 2 id. Optional, only returned if `return_l2dict` is True.
     """
-    DeprecationWarning('This function does not use the L2cache natively and will be moved to pcg_skel.nocache in a future version.')
 
-    if client is None:
-        client = CAVEclient(datastack_name)
-    if n_parallel is None:
-        n_parallel = 1
-    if cv is None:
-        cv = client.info.segmentation_cloudvolume(progress=True, parallel=1)
-
-    if root_point_resolution is None:
-        root_point_resolution = cv.mip_resolution(0)
-
-    (
-        sk_ch,
-        mesh_ch,
-        (l2dict, l2dict_r),
-        (l2dict_mesh, l2dict_mesh_r),
-    ) = chunk_index_skeleton(
-        root_id,
-        client=client,
-        datastack_name=datastack_name,
-        cv=cv,
-        root_point=root_point,
-        root_point_resolution=root_point_resolution,
-        root_point_search_radius=root_point_search_radius,
-        invalidation_d=invalidation_d,
-        return_mesh=True,
-        return_mesh_l2dict=True,
-        return_l2dict=True,
-        n_parallel=n_parallel,
+    warnings.warn(
+        "The function `coord_space_mesh` is deprecated and has been replaced with 'pcg_graph'",
+        DeprecationWarning,
     )
-    if refine == "all":
-        refine_inds = "all"
-    elif refine == "bp":
-        refine_inds = sk_ch.branch_points_undirected
-    elif refine == "ep":
-        refine_inds = sk_ch.end_points_undirected
-    elif refine == "epbp" or refine == "bpep":
-        refine_inds = np.concatenate(
-            (sk_ch.end_points_undirected, sk_ch.branch_points_undirected)
-        )
-    elif refine == "chunk":
-        refine_inds = None
-    elif refine is None:
-        refine_inds = None
-    else:
-        raise ValueError(
-            '"refine" must be one of "all", "bp", "ep", "epbp"/"bpep", "chunk", or None'
-        )
-
-    if root_point is not None:
-        root_point_euc = root_point * np.array([root_point_resolution])
-    else:
-        root_point_euc = None
-
-    sk_l2, missing_ids = refine_chunk_index_skeleton(
-        sk_ch,
-        l2dict_r,
+    return pcg_graph(
+        root_id,
+        client,
         cv=cv,
-        refine_inds=refine_inds,
-        scale_chunk_index=True,
-        root_location=root_point_euc,
+        return_l2dict=return_l2dict,
         nan_rounds=nan_rounds,
-        return_missing_ids=True,
-        segmentation_fallback=segmentation_fallback,
-        fallback_mip=fallback_mip,
-        cache=cache,
-        save_to_cache=save_to_cache,
-        client=client,
-        l2cache=l2cache,
+        require_complete=require_complete,
     )
 
-    if refine == "chunk" or refine is None:
-        refinement_method = None
-    elif segmentation_fallback:
-        refinement_method = "mesh_average_with_seg_fallback"
-    else:
-        refinement_method = "mesh_average"
-    metameta = {
-        "refinement": refine,
-        "refinement_method": refinement_method,
-        "nan_rounds": nan_rounds,
-    }
-    try:
-        sk_l2.meta.update_metameta(metameta)
-    except:
-        pass
-
-    if collapse_soma and root_point is not None:
-        sk_l2 = collapse_pcg_skeleton(
-            sk_l2.vertices[sk_l2.root], sk_l2, collapse_radius
-        )
-
-    if refine == "chunk":
-        sk_l2._rooted._vertices = utils.nm_to_chunk(sk_l2.vertices, cv)
-        try:
-            sk_l2.meta.update_metameta({"space": "chunk"})
-        except:
-            pass
-
-    output = [sk_l2]
-    if return_mesh:
-        output.append(mesh_ch)
-    if return_l2dict:
-        output.append((sk_utils.propagate_l2dict(sk_l2, l2dict_mesh), l2dict_r))
-    if return_l2dict_mesh:
-        output.append((l2dict_mesh, l2dict_mesh_r))
-    if return_missing_ids:
-        output.append(missing_ids)
-    if len(output) == 1:
-        return output[0]
-    else:
-        return tuple(output)
-
-
 
-
-def pcg_meshwork(
+def coord_space_meshwork(
     root_id,
     datastack_name=None,
     client=None,
     cv=None,
-    refine="all",
     root_point=None,
     root_point_resolution=None,
-    root_point_search_radius=300,
     collapse_soma=False,
     collapse_radius=DEFAULT_COLLAPSE_RADIUS,
     synapses=None,
     synapse_table=None,
     remove_self_synapse=True,
     live_query=False,
     timestamp=None,
-    invalidation_d=3,
-    segmentation_fallback=False,
-    fallback_mip=2,
-    cache=None,
-    save_to_cache=False,
-    n_parallel=None,
-    l2cache=False,
+    invalidation_d=DEFAULT_INVALIDATION_D,
+    require_complete=False,
+    metadata=False,
 ):
     """Generate a meshwork file based on the level 2 graph.
 
     Parameters
     ----------
     root_id : int
         Root id of an object in the pychunkedgraph.
     datastack_name : str or None, optional
         Datastack name to use to initialize a client, if none is provided. By default None.
     client : caveclient.CAVEclientFull or None, optional
         Initialized CAVE client. If None is given, will use the datastack_name to create one. By default None
     cv : cloudvolume.CloudVolume or None, optional
         Initialized cloudvolume. If none is given, the client info will be used to create one. By default None
-    refine : 'all', 'ep', 'bp', 'epbp'/'bpep', or None, optional
-        Selects how to refine vertex locations by downloading mesh chunks.
-        Unrefined vertices are placed in the center of their chunk in euclidean space.
-        * 'all' refines all vertex locations. (Default)
-        * 'ep' refines end points only
-        * 'bp' refines branch points only
-        * 'bpep' or 'epbp' refines both branch and end points.
-        * 'chunk' keeps vertices in chunk index space.
-        * None refines no points but maps them to the center of the chunk in euclidean space.
     root_point : array-like or None, optional
         3 element xyz location for the location to set the root in units set by root_point_resolution,
         by default None. If None, a distal tip is selected.
     root_point_resolution : array-like, optional
         Resolution in euclidean space of the root_point, by default [4, 4, 40]
-    root_point_search_radius : int, optional
-        Distance in euclidean space to look for segmentation when finding the root vertex, by default 300
     collapse_soma : bool, optional,
         If True, collapses vertices within a given radius of the root point into the root vertex, typically to better
         represent primary neurite branches. Requires a specified root_point. Default if False.
     collapse_radius : float, optional
         Max distance in euclidean space for soma collapse. Default is 10,000 nm (10 microns).
     synapses : 'pre', 'post', 'all', or None, optional
         If not None, queries the synapse_table for presynaptic synapses (if 'pre'),  postsynaptic sites (if 'post'), or both (if 'all'). By default None
     synapse_table : str, optional
         Name of the synapse table to query if synapses are requested, by default None
     remove_self_synapse : bool, optional
         If True, filters out synapses whose pre- and postsynaptic root ids are the same neuron, by default True
+    live_query : bool, optional
+        If True, expect a timestamp for querying at a give point in time. Otherwise, use the materializatio set by the client. Optional, by default False.
+    timestamp = datetime.datetime, optional
+        If set, acts as the time at which all root ids and annotations are found at.
     invalidation_d : int, optional
         Invalidation radius in hops for the mesh skeletonization along the chunk adjacency graph, by default 3
-    cache : str or None, optional
-        If set to 'service', uses the online l2cache service (if available). Otherwise, this is the filename of a sqlite database with cached lookups for l2 ids. Optional, default is None.
-    n_parallel : int, optional
-        Number of parallel downloads passed to cloudvolume, by default 1
-    l2cache : bool, optional
-        Set to True to use the l2cache. Equivalent to cache='service'.
+    require_complete : bool, optional
+        If True, raise an Exception if any vertices are missing from the cache, by default False
 
     Returns
     -------
     meshparty.meshwork.Meshwork
         Meshwork object with skeleton based on the level 2 graph. See documentation for details.
     """
-    DeprecationWarning('This function does not use the L2cache natively and will be moved to pcg_skel.nocache in a future version.')
-
-    if client is None:
-        client = CAVEclient(datastack_name)
-    if n_parallel is None:
-        n_parallel = 1
-    if cv is None:
-        cv = client.info.segmentation_cloudvolume(progress=True, parallel=1)
-    if root_point_resolution is None:
-        root_point_resolution = cv.mip_resolution(0)
+    warnings.warn(
+        "The function `coord_space_meshwork` is deprecated and has been replaced with 'pcg_meshwork'",
+        DeprecationWarning,
+    )
 
-    sk_l2, mesh_chunk, (l2dict_mesh, l2dict_mesh_r) = pcg_skeleton(
+    return pcg_meshwork(
         root_id,
+        datastack_name=datastack_name,
         client=client,
         cv=cv,
         root_point=root_point,
         root_point_resolution=root_point_resolution,
-        root_point_search_radius=root_point_search_radius,
         collapse_soma=collapse_soma,
         collapse_radius=collapse_radius,
-        refine=refine,
+        synapses=synapses,
+        synapse_table=synapse_table,
+        remove_self_synapse=remove_self_synapse,
+        live_query=live_query,
+        timestamp=timestamp,
         invalidation_d=invalidation_d,
-        n_parallel=n_parallel,
-        return_mesh=True,
-        return_l2dict_mesh=True,
-        segmentation_fallback=segmentation_fallback,
-        fallback_mip=fallback_mip,
-        cache=cache,
-        save_to_cache=save_to_cache,
-        l2cache=l2cache,
+        require_complete=require_complete,
+        metadata=metadata,
     )
-
-    nrn = meshwork.Meshwork(mesh_chunk, seg_id=root_id, skeleton=sk_l2)
-
-    if synapses is not None and synapse_table is not None:
-        if synapses == "pre":
-            pre, post = True, False
-        elif synapses == "post":
-            pre, post = False, True
-        elif synapses == "all":
-            pre, post = True, True
-        else:
-            raise ValueError('Synapses must be one of "pre", "post", or "all".')
-
-        if not timestamp:
-            timestamp = client.materialize.get_timestamp()
-
-        features.add_synapses(
-            nrn,
-            synapse_table,
-            l2dict_mesh,
-            client,
-            root_id=root_id,
-            pre=pre,
-            post=post,
-            remove_self_synapse=remove_self_synapse,
-            timestamp=timestamp,
-            live_query=live_query,
-        )
-
-    features.add_lvl2_ids(nrn, l2dict_mesh)
-
-    if refine != "chunk":
-        chunk_tools.adjust_meshwork(nrn, cv)
-
-    return nrn
-
-
-
-
-def collapse_pcg_skeleton(soma_pt, sk, soma_r):
-    """Use soma point vertex and collapse soma as sphere
-    Parameters
-    ----------
-    soma_pt : array
-        3-element location of soma center (in nm)
-    sk: skeleton.Skeleton
-        Coarse skeleton
-    soma_r : float
-        Soma collapse radius (in nm)
-    Returns
-    -------
-    skeleton
-        New skeleton with updated properties
-    """
-    soma_verts, _ = skeletonize.soma_via_sphere(soma_pt, sk.vertices, sk.edges, soma_r)
-    min_soma_vert = np.argmin(np.linalg.norm(sk.vertices[soma_verts] - soma_pt, axis=1))
-    root_vert = soma_verts[min_soma_vert]
-
-    (
-        new_v,
-        new_e,
-        new_skel_map,
-        vert_filter,
-        root_ind,
-    ) = skeletonize.collapse_soma_skeleton(
-        soma_verts[soma_verts != root_vert],
-        soma_pt,
-        sk.vertices,
-        sk.edges,
-        sk.mesh_to_skel_map,
-        collapse_index=root_vert,
-        return_soma_ind=True,
-        return_filter=True,
-    )
-
-    new_mesh_index = sk.mesh_index[vert_filter]
-    new_skeleton = skeleton.Skeleton(
-        new_v,
-        new_e,
-        root=root_ind,
-        mesh_to_skel_map=new_skel_map,
-        mesh_index=new_mesh_index,
-        remove_zero_length_edges=False,
-        meta=sk.meta,
-    )
-
-    new_skeleton.meta.soma_pt_x = soma_pt[0]
-    new_skeleton.meta.soma_pt_y = soma_pt[1]
-    new_skeleton.meta.soma_pt_z = soma_pt[2]
-    new_skeleton.meta.soma_radius = soma_r
-    new_skeleton.meta.collapse_soma = True
-    new_skeleton.meta.collapse_function = "sphere"
-
-    return new_skeleton
```

### Comparing `pcg_skel-0.3.5/pcg_skel/skel_utils.py` & `pcg_skel-1.0.0/pcg_skel/skel_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import numpy as np
 import warnings
 
+import numpy as np
+
 
 def filter_l2dict(sk_ch, l2dict_mesh_r):
     """Converts a reverse level 2 dict for a mesh into one for a skeleton"""
     l2dict_sk_r = {
         ii: l2dict_mesh_r.get(mind, -1) for ii, mind in enumerate(sk_ch.mesh_index)
     }
     l2dict_sk = {v: k for v, k in l2dict_sk_r.items()}
@@ -46,15 +47,14 @@
                     )
         mesh.vertices[nanvinds] = new_verts
 
         nr += 1
     else:
         if np.any(np.isnan(mesh.vertices)):
             print(f"Could not fix all nans after {num_rounds} rounds")
-    pass
 
 
 def fix_nan_verts(sk, num_rounds=20):
     """Replace vertices with locations that are nan with mean of neighbor locations"""
     if num_rounds is None:
         num_rounds = 0
 
@@ -81,22 +81,20 @@
         if not np.any(np.isnan(new_verts[:, 0])):
             break
 
         nr += 1
     else:
         if np.any(np.isnan(sk.vertices)):
             print(f"Could not fix all nans after {num_rounds} rounds")
-    pass
 
 
 def get_centered_mesh(mesh):
     if mesh is None:
         return np.array([np.nan, np.nan, np.nan])
     verts = mesh.vertices
     close_ind = np.argmin(np.linalg.norm(verts - np.mean(verts, axis=0), axis=1))
     return verts[close_ind]
 
 
 def attach_new_skeleton(nrn, new_skeleton):
     nrn._skeleton = new_skeleton
     nrn._recompute_indices()
-    pass
```

### Comparing `pcg_skel-0.3.5/pcg_skel/utils.py` & `pcg_skel-1.0.0/pcg_skel/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from functools import reduce
+
 import numpy as np
 from trimesh import creation
-from functools import reduce
+
 
 def chunk_dims(cv):
     """Gets the size of a chunk in euclidean space
 
     Parameters
     ----------
     cv : cloudvolume.CloudVolume
```

