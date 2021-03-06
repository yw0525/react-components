# react-components

基于 antd 的 react 组件库。

目前已支持以下组件：

- 树形穿梭框（TreeTransfer）

## 树形穿梭框

https://ant.design/components/transfer-cn/

在 antd 树穿梭框原有功能的基础上，增加以下功能：

- 增加树结点数据懒加载支持；
  - 可默认展示一级结点，点击展开，动态加载子结点。
- 增加远程搜索支持；
  - 已选中树结点，如果更改筛选条件，也可正常在右列表展示（缓存处理）；
  - 编辑时，可正常回显未在左侧搜索列表中的数据；
  - 针对缓存，使用 LRU 缓存淘汰算法进行优化处理。
- 针对选择多级类目等业务场景，增加对已选中树结点的优化处理。
  - 选择所有子级结点，默认选中其父节点；
  - 如果没有选中所有子节点，父节点不会被选中。
