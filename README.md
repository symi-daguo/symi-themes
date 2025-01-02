# SYMI Themes

[![hacs_badge](https://img.shields.io/badge/HACS-Custom-orange.svg)](https://github.com/custom-components/hacs)
[![ha_version](https://img.shields.io/badge/Home%20Assistant-2025.1.2-blue.svg)](https://www.home-assistant.io)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub Release][releases-shield]][releases]
[![GitHub Activity][commits-shield]][commits]

[releases-shield]: https://img.shields.io/github/release/symi-daguo/symi-themes.svg
[releases]: https://github.com/symi-daguo/symi-themes/releases
[commits-shield]: https://img.shields.io/github/commit-activity/y/symi-daguo/symi-themes.svg
[commits]: https://github.com/symi-daguo/symi-themes/commits/main

一套为 Home Assistant 设计的现代化主题集合，专注于现代设计趋势。

## 主题预览

### 1. Neo Minimalist（新极简主义）
- 特点：极简设计，大量留白，高对比度
- 适用场景：追求简约清爽的用户
- 支持：亮色/暗色模式
- 风格：类似iOS/MacOS设计语言
- 主色调：蓝色系 (#007AFF)

### 2. Cyber Neon（赛博霓虹）
- 特点：霓虹色彩，玻璃拟态设计
- 适用场景：科技感强烈的智能家居
- 支持：亮色/暗色模式
- 风格：赛博朋克2077风格
- 主色调：霓虹蓝 (#00F3FF) + 霓虹粉 (#FF00E5)

### 3. Nature Tech（自然科技）
- 特点：自然色彩搭配，生态友好
- 适用场景：智能家居中的环保监测
- 支持：亮色/暗色模式
- 风格：生态环保+科技感
- 主色调：自然绿 (#4CAF50)

### 4. Crystal Clear（水晶透明）
- 特点：全透明设计，毛玻璃效果
- 适用场景：喜欢清透风格的用户
- 支持：亮色/暗色模式
- 风格：Windows 11风格
- 主色调：透明蓝 (rgba(0, 120, 212, 0.9))

### 5. Smart Office（智能办公）
- 特点：专业商务风格，高效清晰
- 适用场景：办公环境的智能控制
- 支持：亮色/暗色模式
- 风格：类似Microsoft 365设计语言
- 主色调：商务蓝 (#0078D4)

## 设备支持列表

### 基础设备
- 灯光控制 (Light)
- 空调/温控 (Climate)
- 窗帘/门 (Cover)
- 媒体播放器 (Media Player)

### 传感器设备
- 温度传感器 (Temperature Sensor)
- 湿度传感器 (Humidity Sensor)
- 空气质量传感器 (Air Quality Sensor)
- 运动传感器 (Motion Sensor)
- 门窗传感器 (Door Sensor)

### 安防设备
- 警报器 (Alarm Control Panel)
  - 在家警戒
  - 离家警戒
  - 触发状态
- 摄像头 (Camera)
- 门锁 (Lock)

### 能源监测
- 电量监测 (Power Sensor)
- 能源消耗 (Energy Sensor)
- 用水监测 (Water Sensor)
- 太阳能系统 (Solar Sensor)

### 自动化设备
- 自动化 (Automation)
- 场景 (Scene)
- 脚本 (Script)

### 其他设备
- 风扇 (Fan)
- 扫地机器人 (Vacuum)
- 加湿器 (Humidifier)
- 开关 (Switch)
- 布尔输入 (Input Boolean)

## 安装方法

### HACS 安装（推荐）
1. 确保已安装 HACS
2. 在 HACS 中添加自定义仓库：
   - 仓库地址：`https://github.com/symi-daguo/symi-themes`
   - 类别选择：Themes
3. 在 HACS 的 Themes 分类中找到 "SYMI Themes"
4. 点击下载
5. 重启 Home Assistant

### 手动安装
1. 下载主题文件
2. 将 `themes` 文件夹复制到 Home Assistant 配置目录
3. 在 `configuration.yaml` 中添加：
```yaml
frontend:
  themes: !include_dir_merge_named themes
```
4. 重启 Home Assistant

## 主题特性

### 通用功能
- 支持明暗模式自动切换
- 适配所有 Home Assistant 标准卡片
- 针对不同设备状态优化显示效果
- 支持主流浏览器
- 响应式设计

### 设备状态显示优化
每个主题都针对不同类型的设备状态进行了专门的颜色优化，确保：
- 状态一目了然
- 色彩协调统一
- 符合直觉的颜色映射
- 清晰的状态区分

## 更新日志

### v1.0.0 (2025-01-02)
- 首次发布
- 包含5个主题
- 支持明暗模式
- 优化移动端显示
- 全面支持各类设备状态显示

## 贡献指南

欢迎提交 Issue 和 Pull Request 来帮助改进主题。

## 许可证

MIT License

## 支持

如果遇到问题，请在 [GitHub Issues](https://github.com/symi-daguo/symi-themes/issues) 中提出。 