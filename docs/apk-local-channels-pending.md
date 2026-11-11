# APK 地方频道补录说明

从 `ΠTV_1.3.4.4.apk` 的 `assets/channel_catalog.json` 与当前源码频道表按频道名比较后，整理出 41 条新增频道记录。

## 已合并到主频道表

以下 4 个频道使用当前源码已支持的解析器，已加入 `app/src/main/assets/channel_catalog.json`：

- 湖南电视剧（MGTV）
- 五星体育、新闻综合、哈哈炫动（KANKANEWS）

上海现有的魔都眼和新纪实编号调整为 405、406，与 APK 的频道序号一致，避免和新增的五星体育编号冲突。

## 待接入频道

其余 37 条记录保存在 `app/src/main/assets/apk_local_channels.json`，该文件是参考数据，不会被应用自动加载。它们属于 CZTV、HNTV、HNNTV、FENGSHOWS、MIGU 等解析类型，当前公开源码没有相应的 resolver；未实现并验证解析器前，不应放进活动频道目录。
