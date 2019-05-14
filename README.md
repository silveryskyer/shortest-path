# shape数据python最短路径分析（shortest-path）
参加的一个比赛的最短路径分析的Python代码，虽然没有获得好的名次 = =

代码都在dijkstraPath文件中，加载的数据分别为为shapefile点和面数据读取方式为：
import geopandas
import matplotlib.pyplot as plt
%matplotlib inline

n_path = 'yourpath/nodes.shp' 

node_shp_df = geopandas.GeoDataFrame.from_file(n_path) #读取nodes.shp数据                                                                                                                                                                                                         e_path = 'yourpath/edges.shp'
edge_shp_df = geopandas.GeoDataFrame.from_file(e_path) #读取edges.shp数据

点数据为包含：
---'geometry'字段：经纬度坐标
---'osmid'字段：点号

面数据包含：
---'from'字段：路径起点
---'to'字段：路径终点
---'maxtime'字段：该条路径消耗的最长时间


