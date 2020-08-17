# AwesomeCesium
本项目列出了与Cesium相关的各种资源。

Awesome lists about all kinds of cesium related resources.

## 1 Data Processing 数据处理

### 1.1 Terrain Building 地形生产

+ [cesium-terrain-builder](https://github.com/geo-data/cesium-terrain-builder). 基于C++的Cesium地形瓦片创建工具库及相关命令行工具。A C++ library and associated command line tools designed to create terrain tiles for use in the Cesium JavaScript library.
+ [ctb-quantized-mesh](https://github.com/ahuarte47/cesium-terrain-builder/tree/master-quantized-mesh). cesium-terrain-builder的一个分支，支持离散网格（不规则三角网）格式地形瓦片的生成。TIN格式地形瓦片与高度图（规则格网）地形瓦片的文件结构相同，但是对于大范围地形渲染具有更高的效率。A branch of cesium-terrain-builder to generate quantized-mesh format cesium terrain tiles. The quantized-mesh format follows the same tile structure as heightmap tiles, but each tile is better optimised for large-scale terrain rendering.
+ [Cesium Terrain Server](https://github.com/geo-data/cesium-terrain-server).一个可以将Cesium地形瓦片进行文件发布的一个服务端程序。瓦片发布后，在客户端中可通过CesiumTerrainProvider进行接入使用。A basic server for serving up filesystem based tilesets representing Cesium.js terrain models. The resources served up are intended for use with the CesiumTerrainProvider JavaScript class present in the Cesium.js client.