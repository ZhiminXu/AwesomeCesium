# AwesomeCesium

Awesome lists about all kinds of cesium related resources.本项目列出了与Cesium相关的各种资源。

## 1 Data Processing 数据处理

### 1.1 Terrain Building 地形生产

+ [cesium-terrain-builder](https://github.com/geo-data/cesium-terrain-builder). A C++ library and associated command line tools designed to create terrain tiles for use in the Cesium JavaScript library. 基于C++的Cesium地形瓦片创建工具库及相关命令行工具。
+ [ctb-quantized-mesh](https://github.com/ahuarte47/cesium-terrain-builder/tree/master-quantized-mesh). A branch of cesium-terrain-builder to generate quantized-mesh format cesium terrain tiles. The quantized-mesh format follows the same tile structure as heightmap tiles, but each tile is better optimised for large-scale terrain rendering. CTB的一个分支，支持离散网格（不规则三角网）格式地形瓦片的生成。离散网格地形瓦片与高度图（规则格网）地形瓦片的文件结构相同，但是对于大范围地形渲染具有更高的效率。
+ [Cesium Terrain Server](https://github.com/geo-data/cesium-terrain-server).A basic server for serving up filesystem based tilesets representing Cesium.js terrain models. The resources served up are intended for use with the CesiumTerrainProvider JavaScript class present in the Cesium.js client. 一个可以将Cesium地形瓦片进行文件发布的服务端程序。瓦片发布后，在客户端中可通过CesiumTerrainProvider进行接入使用。
+ [mbtiles-terrain-server](https://github.com/TNOCS/mbtiles-terrain-server). A mbtiles service that can import millions of small cesium terrain tiles into only a mbtiles (sqlite3) database file and serve them via http. 一个mbtiles服务发布程序，可以将成千上万的Cesium地形瓦片数据导入到一个sqlite数据库文件，并通过http进行发布。

### 1.2 3D Model Converting 三维模型转换

+ [3dtiles](https://github.com/fanvanzh/3dtiles). The so-called fastest tools for 3dtiles converting tool in the world, including osgb-to-3dtiles, shapefile-to-3dtiles and fbx-to-3dtiles converting. 号称世界上最快的 3dtiles 转换工具，支持倾斜摄影数据、shapefile 数据转3dtiles，支持 osg、osgb、obj、fbx、3ds、b3dm等单一通用模型数据转为 gltf、glb 格式。
+ [COLLADA2GLTF](https://github.com/KhronosGroup/COLLADA2GLTF). A command-line tool to convert COLLADA (.dae) files to glTF supporting Windows, MacOS, and Linux. 一个将COLLADA（.dae格式）模型转换为gltf格式的命令行工具，支持Windows、MacOS和Linux。
+ [gltf-to-3dtiles](https://github.com/nxddsnc/gltf-to-3dtiles). A command line tool to convert gltf(glb) file to 3d tiles format.一个将gltf或glb格式转化为3dtiles的命令行工具。
+ [obj2gltf](https://github.com/CesiumGS/obj2gltf).  Node command line tool to convert OBJ assets to glTF 2.0. 将obj格式文件转换为gltf 2.0格式的Node命令行工具。
+ [objTo3d-tiles](https://github.com/PrincessGod/objTo3d-tiles). Node command line tool and module convert obj model file to 3D Tiles, based on [obj2gltf](https://github.com/CesiumGS/obj2gltf). 基于[obj2gltf](https://github.com/CesiumGS/obj2gltf), 将obj模型文件转换为3dtiles格式的Node命令行工具
+ [citygml-to-3dtiles](https://github.com/njam/citygml-to-3dtiles). A very basic and experimental converter from CityGML to Cesium 3D Tiles. 一个将CityGML格式转化为3dtiles的**基础实验性**命令行工具。