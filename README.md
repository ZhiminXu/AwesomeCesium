# AwesomeCesium

Awesome lists about all kinds of cesium related resources.本项目列出了与Cesium相关的各种资源。

## 1 Data Processing 数据处理

### 1.1 Terrain Building 地形生产

+ [cesium-terrain-builder](https://github.com/geo-data/cesium-terrain-builder). A C++ library and associated command line tools designed to create terrain tiles for use in the Cesium JavaScript library. 基于C++的Cesium地形瓦片创建工具库及相关命令行工具。
+ [ctb-quantized-mesh](https://github.com/ahuarte47/cesium-terrain-builder/tree/master-quantized-mesh). A branch of cesium-terrain-builder to generate quantized-mesh format cesium terrain tiles. The quantized-mesh format follows the same tile structure as heightmap tiles, but each tile is better optimised for large-scale terrain rendering. CTB的一个分支，支持离散网格（不规则三角网）格式地形瓦片的生成。离散网格地形瓦片与高度图（规则格网）地形瓦片的文件结构相同，但是对于大范围地形渲染具有更高的效率。
+ [gdal2cesium](https://github.com/giohappy/gdal2cesium). A Python command line utility, based on GDAL and inspired by gdal2tiles, to generate terrain heightmap tiles accordig to the native Cesium format. 基于GDAL的Python命令行工具，可以生产高度图格式的Cesium地形数据。
+ [Cesium Terrain Server](https://github.com/geo-data/cesium-terrain-server).A basic server for serving up filesystem based tilesets representing Cesium.js terrain models. The resources served up are intended for use with the CesiumTerrainProvider JavaScript class present in the Cesium.js client. 一个可以将Cesium地形瓦片进行文件发布的服务端程序。瓦片发布后，在客户端中可通过CesiumTerrainProvider进行接入使用。
+ [mbtiles-terrain-server](https://github.com/TNOCS/mbtiles-terrain-server). A mbtiles service that can import millions of small cesium terrain tiles into only a mbtiles (sqlite3) database file and serve them via http. 一个mbtiles服务发布程序，可以将成千上万的Cesium地形瓦片数据导入到一个sqlite数据库文件，并通过http进行发布。

### 1.2 3D Model Converting 三维模型转换

+ [3dtiles](https://github.com/fanvanzh/3dtiles). The so-called fastest tools for 3dtiles converting tool in the world, including osgb-to-3dtiles, shapefile-to-3dtiles and fbx-to-3dtiles converting. 号称世界上最快的 3dtiles 转换工具，支持倾斜摄影数据、shapefile 数据转3dtiles，支持 osg、osgb、obj、fbx、3ds、b3dm等单一通用模型数据转为 gltf、glb 格式。
+ [COLLADA2GLTF](https://github.com/KhronosGroup/COLLADA2GLTF). A command-line tool to convert COLLADA (.dae) files to glTF supporting Windows, MacOS, and Linux. 一个将COLLADA（.dae格式）模型转换为gltf格式的命令行工具，支持Windows、MacOS和Linux。
+ [gltf-to-3dtiles](https://github.com/nxddsnc/gltf-to-3dtiles). A command line tool to convert gltf(glb) file to 3d tiles format.一个将gltf或glb格式转化为3dtiles的命令行工具。
+ [obj2gltf](https://github.com/CesiumGS/obj2gltf).  Node command line tool to convert OBJ assets to glTF 2.0. 将obj格式文件转换为gltf 2.0格式的Node命令行工具。
+ [objTo3d-tiles](https://github.com/PrincessGod/objTo3d-tiles). Node command line tool and module convert obj model file to 3D Tiles, based on [obj2gltf](https://github.com/CesiumGS/obj2gltf). 基于[obj2gltf](https://github.com/CesiumGS/obj2gltf), 将obj模型文件转换为3dtiles格式的Node命令行工具
+ [citygml-to-3dtiles](https://github.com/njam/citygml-to-3dtiles). A very basic and experimental converter from CityGML to Cesium 3D Tiles. 一个将CityGML格式转化为3dtiles的**基础实验性**命令行工具。
+ [cesium_pnt_generator](https://github.com/mattshax/cesium_pnt_generator). Convert lidar las datasets into Cesium pnts 3d-tiles. 将las点云数据集转换为3dtiles格式。

## 2 Front-end Framework Integration 前端框架集成

### 2.1 Angular
+ [cesium-angular-example](https://github.com/Developer-Plexscape/cesium-angular-example). A simple web application that demonstrates integration of Cesium with the LATEST version of Angular. 一个简单的web应用程序，演示了Cesium与最新版的Angular的集成。
+ [angular-cesium](https://github.com/articodeltd/angular-cesium). JavaScript library for creating map based web apps using Cesium and Angular, which is an angular wrapper for cesium.js. 使用Cesium与Angular创建地图Web应用的JavaScript库，基于Angular对cesium.js进行了封装。

### 2.2 Vue
+ [cesium-vue](https://github.com/ShareQiu1994/cesium-vue). Cesium development template based on vueCli 4.x.x +. 基于vueCli 4.x.x + 的cesium开发模板.
+ [vue-cesium](https://github.com/zouyaoji/vue-cesium). Vue 2.x components for CesiumJS. Load Cesium built package or other third-party packages which are built on Cesium. 基于 Vue2.x的 Cesium 三维地图组件,

### 2.3 React
+ [resium](https://github.com/darwin-education/resium). React components for Cesium. 基于React封装的Cesium组件库。
+ [cesium_demos](https://github.com/NichijouCC/cesium_demos). Demo applications based on cesium, react and typescript. 使用cesium+react+ts编写的cesium使用样例程序库。

## 3 Cesium Extension Cesium功能扩展

### 3.1 Provider 数据驱动

+ [CesiumVectorTile](https://github.com/MikesWei/CesiumVectorTile). Vector Tile Imagery Provider for Cesium. 实现将geojson、shp等矢量数据动态切片贴地的Cesium驱动。
+ [WCSTerrainProvider](https://github.com/xlhomme/WCSTerrainProvider). WCS Terrain Provider for Cesium. 添加WCS地形的Cesium驱动。
+ [Cesium-GeoserverTerrainProvider](https://github.com/kaktus40/Cesium-GeoserverTerrainProvider). A terrain provider which works with geoserver providing elevation datas in bil, png, gif and jpeg formats. 将Geoserver作为地形驱动的插件。

### 3.2 UI 界面元素

+ [cesium-navigation](https://github.com/alberto-acevedo/cesium-navigation). Cesium plugin that adds to the Cesium map a compass, navigator (zoom in/out), and distance scale. 可以给Cesium地图添加罗盘、地图缩放、比例尺等工具条的插件。

### 3.3 Data Visualization 数据展示
+ [CesiumHeatmap](https://github.com/manuelnas/CesiumHeatmap). A library to add heatmaps (using heatmap.js) to the Cesium framework. 使用HeatMap.js 向Cesium地图添加热力图的扩展库。
+ [3D-Wind-Field](https://github.com/RaymanNg/3D-Wind-Field). Visualize wind field on Cesium. 基于Cesium实现三维环境下风场数据的可视化。
+ [Wind-Field-Cesium](https://github.com/AlbertEjiestein/Wind-Field-Cesium). Visualize the wind on earth, powered by Cesium JS. 基于Cesium实现三维环境下风场数据的可视化，在[3D-Wind-Field](https://github.com/RaymanNg/3D-Wind-Field)这个项目的基础上添加了颜色表配置，可实现彩色的风场可视化。
+ [d3cesium](https://github.com/abwood/d3cesium). Demo web app featuring Cesium and d3 libraries. 基于Cesium与D3.js结合的示例程序。
+ [CesiumMeshVisualizer](https://github.com/MikesWei/CesiumMeshVisualizer). Make you can use three.js geometry in Cesium,and use mesh,geometry,material like three.js to manage renderable object in Cesium. 可以让你在Cesium中使用three.js对可渲染对象的三角网、几何、材质等信息进行管理。
+ [ol-cesium](https://github.com/openlayers/ol-cesium). OpenLayers - Cesium integration library. Create your map using OpenLayers, and visualize it on a globe with Cesium. OpenLayer与Cesium的继承库，可以让你使用OpenLayers创建二维地图并在Cesium中进行可视化。
+ [cesium-vr](https://github.com/NICTA/cesium-vr). Plugin for Cesium web-based virtual globe software to support the Oculus VR headset. Cesium的VR插件，支持将web端数字地球接入Oculus头盔中显示。

### 3.4 Editor 编辑功能
+ [cesium-drawhelper](https://github.com/leforthomas/cesium-drawhelper). A very early stage shape editor for Cesium. Currently limited to 2D and simple shapes. Cesium矢量编辑工具，早期版本，目前仅限于二维与简单矢量的编辑。

## 4 Cesium based 3DGIS SDK 基于Cesium的三维GIS开发包
+ [dc-sdk](https://github.com/dvgis/dc-sdk). DC-SDK is based on the open source project Cesium for the second development of two three-dimensional WebGis application framework , the framework optimizes the use of Cesium and adds some additional features , designed for developers to quickly build WebGis application. DC-SDK 是基于Cesium的三维WebGIS开发框架，该框架优化了Cesium的部分功能，并补充了一些新特定，可辅助开发者进行WebGIS应用的快速搭建。
+ [mars3d](https://github.com/marsgis/mars3d). Mars3d 3D Earth platform is a B/S architecture 3D client development platform developed by Mars Technology based on webgl and cesium, which supports multi industry applications. Mars3D 三维地球平台软件是火星科技研发的一款基于 WebGL、Cesium优化提升的B/S架构三维客户端开发平台，支持多行业扩展应用。

## 5 Demos 示例程序
+ [Cesium.HPUZYZ.Demo](https://github.com/YanzheZhang/Cesium.HPUZYZ.Demo).This project is some demos of CESIUM. Much of them are from other people's blogs and cesium's official website. Thanks to my good friend [MikesWei](https://github.com/MikesWei) for giving me great help. 这个项目整理了基于Cesium的各种示例程序，大部分都是来自于其他人的博客和Cesium官方网站。感谢 [MikesWei](https://github.com/MikesWei)给我的巨大帮助。
+ [CesiumJS-tutorial](https://github.com/hujiulin/CesiumJS-tutorial).Offical tutorial from Cesium Chinese Website ( http://cesiumcn.org/ | http://cesium.coinidea.com/ ). [Cesium中文网](http://cesiumcn.org/)官网教程。