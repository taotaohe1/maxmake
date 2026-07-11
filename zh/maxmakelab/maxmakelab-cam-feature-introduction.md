# MaxmakeLab CAM功能介绍页面

MaxmakeLAB-0.9.18版本更新，新增了CAM相关功能：毛坯设置，刀具库管理，轮廓铣、平面铣、浮雕加工三种刀具策略，仿真功能。以下是各个功能的介绍

## 1. 毛坯设置（Job Step）

<img src="/chi/maxmakelab/media/maxmakelab-cam-feature-introduction/毛坯设置.webp" alt="毛坯设置演示" style="width: 100%; height: auto; margin-bottom: 4px; border-radius: 16px;" />

- 可设置毛坯的长宽高
- 加工起点目前默认为顶点，后续会增加底面为零点功能
- 可设置原点：中心点或左下角点
- 可设置加工安全高度

## 2. 刀具库（Tool Library）

<img src="/chi/maxmakelab/media/maxmakelab-cam-feature-introduction/刀具库.webp" alt="刀具库演示" style="width: 100%; height: auto; margin-bottom: 4px; border-radius: 16px;" />

- 可修改刀具参数如下：
  - 刀具号、单位、直径等
  - 下切步距、步距、主轴转速、进给率、下切速率等
- 可添加组、添加刀具、复制删除刀具或者组

> ⚠️ **注意事项**：
>
> - 导入导出暂时有问题，后续会修复
> - 目前支持平底刀、球头刀、平底尖刀、V型刀。后续会添加其他种类刀具
> - 目前只显示一种材料，后续会增加
>
> {.is-warning}

## 3. 轮廓铣（Profile Toolpath）

<img src="/chi/maxmakelab/media/maxmakelab-cam-feature-introduction/轮廓铣.webp" alt="轮廓铣演示" style="width: 100%; height: auto; margin-bottom: 4px; border-radius: 16px;" />

- 选择矢量后，可生成轮廓路径
- 可设置加工深度，加工起始高度后续添加
- 可选择刀具库里的刀具，并支持临时更改参数，临时更改的参数不会影响刀具库的参数
- 可选择沿矢量外，沿矢量，沿矢量内三种方式
- 可选择顺逆铣
- 斜插功能、桥功能后续添加

## 4. 平面铣（Pocket Toolpath）

<img src="/chi/maxmakelab/media/maxmakelab-cam-feature-introduction/平面铣.webp" alt="平面铣演示" style="width: 100%; height: auto; margin-bottom: 4px; border-radius: 16px;" />

- 选择矢量后，可生成平面铣路径
- 可设置加工深度，加工起始高度后续添加
- 可选择刀具库里的刀具，并支持临时更改参数，临时更改的参数不会影响刀具库的参数
- 斜插功能、第二把刀铣残料功能后续添加

## 5. 浮雕加工（Relief Toolpath）

<img src="/chi/maxmakelab/media/maxmakelab-cam-feature-introduction/浮雕加工.webp" alt="浮雕加工演示" style="width: 100%; height: auto; margin-bottom: 4px; border-radius: 16px;" />

- 选择图片后，可生成浮雕路径
- 可设置加工深度，目前设置后，即为浮雕的高度
- 可选择刀具库里的刀具，并支持临时更改参数，临时更改的参数不会影响刀具库的参数
- 默认按照图形的边缘偏移后进行粗加工，后续增加边界限制选项
- 斜插功能后续添加

> ⚠️ **注意事项**：
>
> - 浮雕功能目前粗加工余量预留的比较多，建议不要在檀木等硬木上加工，后续我们会优化此功能
>
> {.is-warning}

## 6. 仿真（Simulate）

<img src="/chi/maxmakelab/media/maxmakelab-cam-feature-introduction/仿真加工.webp" alt="仿真演示" style="width: 100%; height: auto; margin-bottom: 4px; border-radius: 16px;" />

- 生成路径后，可点击仿真按钮，查看仿真加工效果
- 可打开/关闭路径的显示
- 可调整播放速度，可拖动进度条快速查看
- 拖动时，会存在有路径未渲染的问题，后续会修复

## 7. 导出（Export）

<img src="/chi/maxmakelab/media/maxmakelab-cam-feature-introduction/导出.webp" alt="导出演示" style="width: 100%; height: auto; margin-bottom: 4px; border-radius: 16px;" />

- 生成路径后，可点击导出按钮，导出Gcode，为NC格式
- 连接机器并归零的情况下，可直接导入机器

> ⚠️ **注意事项**：
>
> - 导出时，路径暂时是分散的，建议不要改动，后续我们会优化此功能
> - 因代码始终含有换刀代码T\*M6，需要点击换刀，测高后设置零点，再运行代码
>
> {.is-warning}

## 8. 问题反馈

有任何软件问题，可在Discord软件反馈专区内联系我们。我们会积极参考大家的建议并及时修复问题：

- [Discord](https://discord.com/channels/1436232802227064903/1436232803061600351)