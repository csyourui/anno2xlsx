[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/liserjrqlxue/anno2xlsx)

# anno2xlsx



# 注意
## 基因-疾病数据库
**基因-疾病数据库**属于保密数据库，仅供内部测试使用  
~~后续会通过数据库服务获取或者直接创建加密数据库~~  
已通过aes对json格式进行加密处理

## 突变频谱数据库
**突变频谱数据库**属于保密数据库，仅供内部测试使用，  
~~后续会通过数据库服务获取或者直接创建加密数据库~~  
已通过aes对json格式进行加密处理

## 特殊位点库
**特殊位点库**根据华大内部流程`bgicg_anno.pl`注释结果中的`MutationName`查找是否特殊位点，
所以以下情形可能发生库失效问题：
1. 输入文件不包含以`MutationName`命名的特定注释结果
2. 输入文件`MutationName`与流程`bgicg_anno.pl`结果不一致
3. 流程`bgicg_anno.pl`有更新，但是数据库未同步更新
4. 位点用与现有配置不同的数据库注释导致的注释结果不一致