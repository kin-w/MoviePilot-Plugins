# MoviePilot-Plugins

个人 MoviePilot 插件仓库，当前发布插件：**蛙辅·跳校版**（CrossSeedSkipVerify）。

## 插件列表

| 插件 ID | 名称 | 版本 | 说明 |
| --- | --- | --- | --- |
| `CrossSeedSkipVerify` | 蛙辅·跳校版 | `3.0.4` | 支持 NexusPHP 站点自动辅种，基于“青蛙辅种助手”修改，新增跳过校验（skipverify）与自动开始做种（auto_start）能力。 |

## 版本兼容

- MoviePilot **V1 / V2 / V3** 均可安装。
- 插件为单份跨版本实现：源码位于 `plugins/crossseedskipverify/`，索引位于 `package.json`（声明 `v2: true`）。
- V3 宿主通过官方兼容层加载，无需 V3 专用副本。

## 安装方法

1. 打开 MoviePilot 后台 → **设置** → **插件**（插件仓库 / 插件市场配置项）。
2. 在插件仓库地址中添加本仓库地址：

   ```
   https://github.com/kin-w/MoviePilot-Plugins
   ```

   多个仓库地址时使用英文逗号分隔。
3. 保存后刷新**插件市场**，找到「蛙辅·跳校版」点击安装。
4. 安装后在插件详情页配置下载器、辅种站点、种子目录等参数并启用。

## 仓库结构

```text
MoviePilot-Plugins/
├── plugins/
│   └── crossseedskipverify/     # 插件源码（目录名 = 主类名小写）
│       └── __init__.py
├── icons/
│   └── qingwa.png               # 插件图标
├── package.json                 # 插件市场索引（V1/V2/V3 通用）
└── README.md
```

