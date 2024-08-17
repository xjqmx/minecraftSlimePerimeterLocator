# minecraftSlimePerimeterLocator
一个用于在Java版Minecraft中定位史莱姆农场空置域的建造位置的小工具，它可以在给定的区块范围内定位出单名玩家的刷怪范围（24-128格）内史莱姆区块最多的若干个区域的中心区块坐标，并计算出其对应的可用于生成史莱姆的有效区块和有效方块数量。

## 使用要求
Java编译和运行环境

## 使用方法
1.将源码下载到本地

2.根据情况和需求修改java文件中的以下参数
|参数名                     |示例                         |描述                          |
|---------------------------|----------------------------|------------------------------|
|world_seed                 |3523598249870287597L        |世界种子                       |
|central_chunk_x_start      |-500                        |中心区块X轴检索范围起始坐标      |
|central_chunk_x_end        |500                         |中心区块X轴检索范围终止坐标      |
|central_chunk_z_start      |-500                        |中心区块Z轴检索范围起始坐标      |
|central_chunk_z_end        |500                         |中心区块Z轴检索范围终止坐标      |
|min_slime_chunk_requirement|43                          |最小史莱姆区块数量需求          |

3.编译并运行

## 注意事项
1.请注意程序输出结果中的坐标为区块坐标，不是世界坐标

2.中心区块的(0,~,0)位置（即西北角）为空置域中心点

3.如果编译时报错“错误: 整数太大”，请检查是否忘记了world_seed末尾的“L”
