
# SIFT 算法

### 优点

- 应对旋转、尺度、平移 （RST）
- 图像仿射变化、投影变换 （视角）
- 光照影响，遮挡、噪声

### 原理

#### 高斯模糊
在不同尺度上查找关键点并计算关键点方向，sift所查找到的关键点是不会因光照仿射变换噪声等影响而变化的点

尺度空间的获取需要高斯模糊来完成，高斯核是实现尺度变换的唯一线性核。

高斯函数的delta值越大，图像越模糊，是因为原始像素值具有更大的高斯分布值（权重）