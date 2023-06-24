# Comparing `tmp/genopyc-1.0.6-py3-none-any.whl.zip` & `tmp/genopyc-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 421686 bytes, number of entries: 8
+Zip file size: 424126 bytes, number of entries: 8
 -rwxrwxrwx  2.0 unx      917 b- defN 23-Jun-21 11:24 genopyc/__init__.py
--rwxrwxrwx  2.0 unx    32935 b- defN 23-Jun-21 11:26 genopyc/genopyc.py
+-rwxrwxrwx  2.0 unx    42070 b- defN 23-Jun-24 20:35 genopyc/genopyc.py
 -rwxrwxrwx  2.0 unx  1302100 b- defN 23-Jun-21 11:17 genopyc/data/hippie_interactome.sif
--rwxrwxrwx  2.0 unx    34523 b- defN 23-Jun-21 11:44 genopyc-1.0.6.dist-info/LICENSE.txt
--rwxrwxrwx  2.0 unx      596 b- defN 23-Jun-21 11:44 genopyc-1.0.6.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Jun-21 11:44 genopyc-1.0.6.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        8 b- defN 23-Jun-21 11:44 genopyc-1.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      635 b- defN 23-Jun-21 11:44 genopyc-1.0.6.dist-info/RECORD
-8 files, 1371806 bytes uncompressed, 420586 bytes compressed:  69.3%
+-rwxrwxrwx  2.0 unx    34523 b- defN 23-Jun-24 20:36 genopyc-1.1.0.dist-info/LICENSE.txt
+-rwxrwxrwx  2.0 unx      596 b- defN 23-Jun-24 20:36 genopyc-1.1.0.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Jun-24 20:36 genopyc-1.1.0.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        8 b- defN 23-Jun-24 20:36 genopyc-1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      635 b- defN 23-Jun-24 20:36 genopyc-1.1.0.dist-info/RECORD
+8 files, 1380941 bytes uncompressed, 423026 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: genopyc/genopyc.py
 Comment: 
 
 Filename: genopyc/data/hippie_interactome.sif
 Comment: 
 
-Filename: genopyc-1.0.6.dist-info/LICENSE.txt
+Filename: genopyc-1.1.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: genopyc-1.0.6.dist-info/METADATA
+Filename: genopyc-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: genopyc-1.0.6.dist-info/WHEEL
+Filename: genopyc-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: genopyc-1.0.6.dist-info/top_level.txt
+Filename: genopyc-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: genopyc-1.0.6.dist-info/RECORD
+Filename: genopyc-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## genopyc/genopyc.py

```diff
@@ -831,7 +831,226 @@
     
     EdgeFile=ParseInteractome()
 
     HippieNet = nx.from_pandas_edgelist(EdgeFile)
     SubG = HippieNet.subgraph(ListOfGenes)
     Enrichment = EnrichmentAnalisys(ListOfGenes)
     BuildGraph(SubG,Enrichment)
+
+
+#use this function#
+
+
+def plot_enrichment_analisys_network(df,pvalue,colormap='cividis',edgecolor='red',mkcolor='grey',mkfsize=10000,layout='spring',
+                                     mklinewidths=2,alpha=1,figsize=(40,20),savefig=False,factor=1,k=10,
+                                     cbarfontsize=10,labelling=True,legend=False, legend_fontsize = 20, legend_titlefontsize = 25,
+                                     legend_location = (0.5,0.0), legend_col = 6, legend_labelspacing = 1.5, legend_title = '',
+                                     legend_columnspacing=1.5, legend_handlelength = 3, size_legend_nofelements=3, cbar_orientation= 'horizontal',
+                                     cbar_loc=(1, 0.5),**kwargs):
+    def labelling_without_overlapping(x,y,list_of_annotations,ax,verbose=False,**kwargs):
+    
+        class Point:
+            def __init__(self, x, y):
+                self.x = x
+                self.y = y
+    
+    
+        def doOverlap(ret1,ret2):
+            l1 = Point(ret1[0,0],ret1[1,1])
+            r1 = Point(ret1[1,0],ret1[0,1])
+            l2 = Point(ret2[0,0],ret2[1,1])
+            r2 = Point(ret2[1,0],ret2[0,1])
+
+            # If one rectangle is on left side of other
+            if l1.x >= r2.x or l2.x >= r1.x:
+                return False
+
+            # If one rectangle is above other
+            if(r1.y >= l2.y or r2.y >= l1.y):
+                return False
+
+            return True
+
+    annotations_coord=[]
+    for i, dot in enumerate(y):
+        x_coords=x[i]
+        y_coords=y[i]
+        annotation=ax.annotate(str(list_of_annotations[i]),
+                                xy=(x[i],y[i]),
+                                 xytext=(x_coords,y_coords),
+                                    **kwargs)
+
+        ax.figure.canvas.draw()
+        bbox=matplotlib.text.Text.get_window_extent(annotation)
+        bbox_data = ax.transData.inverted().transform(bbox)
+        factor=0.2*(bbox_data[0,0]-bbox_data[1,0])
+        annotations_coord.append(bbox_data)
+        ##BUILD THE SPIRAL##
+        theta=np.radians(np.linspace(1,360*200,500))
+        r=np.linspace(0,max(max(zip(x,y))),len(theta))
+        x_2 = r*np.cos(theta)+x_coords#move the spiral onto the data point
+        y_2 = r*np.sin(theta)+y_coords
+        n=0
+        keep_cycling=True
+        while keep_cycling:
+            keep_cycling=False
+            if verbose==True:
+                print('start checking box %s'% i)
+            for ind, box in enumerate (annotations_coord[0:-1]):
+                if verbose:
+                    print('checking %s and %s' % (i,ind))
+                if doOverlap(box,bbox_data):
+                    if verbose:
+                        print('%s and %s overlap' % (i,ind))
+                    annotation.set_x(x_2[n])
+                    annotation.set_y(y_2[n])
+                    n+=1
+                    ax.figure.canvas.draw()
+                    bbox=matplotlib.text.Text.get_window_extent(annotation)
+                    bbox_data = ax.transData.inverted().transform(bbox)
+                    annotations_coord.pop()
+                    annotations_coord.append(bbox_data)
+                    if verbose:
+                        print('new coords (x=%i,y=%i)'%(x_coords,y_coords))
+                        print('new bbox data',bbox_data)
+                        print('annotation coordinates',box)
+                        print('restart iteration')
+                    keep_cycling=True
+                    break
+
+
+
+    maxpv=max([-np.log10(p) for p in df.p_value.tolist()])
+    for i, (s,v) in enumerate(zip(df.source.value_counts().index,df.source.value_counts())):
+        data=df[(df.source==s)&(-np.log10(df.p_value)>pvalue)].reset_index()
+        if data.shape[0]==0:
+            continue
+        else:
+            
+            nxen=nx.Graph()
+            #add nodes
+            for i,r in data.iterrows():
+                 nxen.add_node(r['name'],size=r['intersection_size'],pvalue=-np.log10(r['p_value']))
+
+            #add edges
+            for i,r in data.iterrows():
+                for index,row in data.iloc[i+1:].reset_index().iterrows():
+                    if len(set(r['intersections']).intersection(set(row['intersections'])))>0:
+                        nxen.add_edge(r['name'],
+                                    row['name'], 
+                                    weight= len(set(r['intersections']).intersection(set(row['intersections']))))
+            # Get positions for the nodes in G
+            if layout=='spring':
+                pos_ = nx.spring_layout(nxen,k)
+            
+            elif layout=='auto':
+                ig_subgraph=ig.Graph.from_networkx(nxen)
+                pos_= dict(zip([v['_nx_name'] for v in ig_subgraph.vs],[coord for coord in ig_subgraph.layout_auto()]))
+                    
+                    
+
+
+            
+
+            #Normalize connections
+            connections=[]
+            for edge in nxen.edges(data=True):
+                connections.append(edge[2]['weight'])
+            if len(connections)!=0:
+                
+                if ((max(connections)-min(connections)==0) | (len(connections)==0)):
+                    norm_connections=[x/100 for x in connections]
+                else:
+                    norm_connections=[(x-min(connections))/(max(connections)-min(connections)) for x in connections]
+            else:
+                connections=norm_connections
+
+
+            #Normalize sizes
+            markers=[]
+            for node in nxen.nodes(data=True):
+                markers.append(node[1]['size'])
+            if len(markers)!=0:
+                
+                if ((max(markers)-min(markers)==0) | (len(markers)==0)):
+                    norm_markers=[x/100 for x in markers]
+                else:
+                    norm_markers=[(x-min(markers))/(max(markers)-min(markers)) for x in markers]
+            else:
+                markers=norm_markers
+            
+               
+            norm_markers=np.clip(norm_markers,0.3, 1)
+            
+            
+            fig,ax=plt.subplots(figsize=figsize)
+            
+            ##Plot the nodes
+            xses,yses=[],[]
+            lab=[]
+            colors=[]
+            for node in nxen.nodes(data=True):
+                xses.append(pos_[node[0]][0])
+                yses.append(pos_[node[0]][1])
+                lab.append(node[0])
+                colors.append(node[1]['pvalue'])
+            
+            nodez_for_legend = ax.scatter(xses,yses,s=markers)
+            nodez=ax.scatter(xses,yses,s=[mkfsize*size for size in norm_markers],
+                           c=colors,cmap=colormap,vmax=maxpv,alpha=alpha,edgecolors=mkcolor,
+                             linewidths=mklinewidths,clip_on=False,zorder=1)
+
+            ##Mark the labels
+            if labelling:
+                labelling_without_overlapping(xses,yses,lab,ax,**kwargs)
+            
+
+
+            ##Plot the edges
+            for indx, edge in enumerate(nxen.edges(data=True)):
+                if edge[2]['weight'] > 0:
+                    path_1 = edge[0]#prepare the data to insert in make edge
+                    path_2 = edge[1]
+                    x0, y0 = pos_[path_1]
+                    x1, y1 = pos_[path_2]
+                    edgez=ax.plot(np.linspace(x0,x1),np.linspace(y0,y1),
+                            color=edgecolor,
+                            linewidth = 3*norm_connections[indx]**4,
+                                 zorder=0)
+
+
+            cbar=plt.colorbar(nodez,ax=ax,orientation=cbar_orientation,panchor=cbar_loc)
+            cbar.set_label(r'$-log_{10}(p-value)$',fontsize=cbarfontsize+4)
+            cbar.ax.tick_params(labelsize=cbarfontsize)
+            
+            
+            if legend:
+                handles, _ = nodez.legend_elements(prop="sizes", alpha=0.6, num = size_legend_nofelements)
+                _, label_markers = nodez_for_legend.legend_elements(prop="sizes", alpha=0.6)
+
+
+                legend = ax.legend(handles, label_markers,fontsize = legend_fontsize,
+                                    bbox_to_anchor=legend_location,ncol=legend_col,labelspacing = legend_labelspacing,
+                                   columnspacing=legend_columnspacing,handlelength=legend_handlelength,frameon = False)
+
+                legend.set_title(legend_title,prop={'size':legend_titlefontsize})
+
+            ax.spines['right'].set_visible(False)
+            ax.spines['top'].set_visible(False)
+            ax.spines['left'].set_visible(False)
+            ax.spines['bottom'].set_visible(False)
+            ax.set_title(s,fontsize=35)
+            ax.set_xticklabels([])
+            ax.set_yticklabels([])
+            ax.set_xticks([])
+            ax.set_yticks([])
+            axis = plt.gca()
+            # maybe smaller factors work as well, but 1.1 works fine for this minimal example
+            axis.set_xlim([factor*x for x in axis.get_xlim()])
+            axis.set_ylim([factor*y for y in axis.get_ylim()])
+            plt.tight_layout()
+            if savefig:
+                plt.savefig(str(s)+'enrichment_analysis.jpeg', dpi=300,bbox_inches='tight')
+            
+            
+            
+            plt.show()
```

## Comparing `genopyc-1.0.6.dist-info/LICENSE.txt` & `genopyc-1.1.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `genopyc-1.0.6.dist-info/METADATA` & `genopyc-1.1.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genopyc
-Version: 1.0.6
+Version: 1.1.0
 Author: Francesco Gualdi
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests
 Requires-Dist: pandas
 Requires-Dist: numpy
```

