# SYMI Themes

Home Assistant 的现代主题集合

## 主题列表

1. 新极简
   - 基础主题：iOS风格的简约设计
   - 深蓝色变体：采用 iOS 深蓝色调，搭配深色背景
   - 浅绿色变体：清新的浅绿色调，搭配明亮背景
   - 深红色变体：热情的深红色调，搭配暗色背景
2. 智能办公：专为办公环境优化的主题
3. 自然科技：结合自然元素和科技感的主题
4. 水晶透明：通透清晰的玻璃拟态设计
5. 赛博霓虹：充满未来感的霓虹风格
6. 赛博朋克2077：赛博朋克风格主题

## 特点

- 基于 iOS 设计语言，提供统一的视觉体验
- 完整支持浅色/深色模式自动切换
- 丰富的动画效果和过渡
- 优化的设备状态显示和控制界面
- 多种主题变体，满足不同场景需求
- 精心设计的卡片布局和间距
- 优化的移动端显示效果
- 自适应的字体大小和颜色对比度

## 安装

### HACS (推荐)

1. 打开 HACS
2. 点击集成
3. 点击右上角的 ⋮ 按钮
4. 选择自定义存储库
5. 输入 https://github.com/symi-daguo/symi-themes
6. 选择类别为 Theme
7. 点击添加
8. 点击安装

### 手动安装

1. 下载此仓库
2. 将 `themes` 文件夹复制到您的 Home Assistant 配置目录
3. 在 `configuration.yaml` 中添加:

```yaml
frontend:
  themes: !include_dir_merge_named themes
```

4. 重启 Home Assistant

## 使用

1. 打开 Home Assistant
2. 点击您的用户头像
3. 选择主题
4. 从下拉菜单中选择您喜欢的主题

### 自动切换

您可以设置在特定时间自动切换主题，例如：

```yaml
automation:
  - alias: '日间主题'
    trigger:
      platform: sun
      event: sunrise
    action:
      service: frontend.set_theme
      data:
        name: 新极简-浅绿

  - alias: '夜间主题'
    trigger:
      platform: sun
      event: sunset
    action:
      service: frontend.set_theme
      data:
        name: 新极简-深蓝
```

## 自定义

每个主题都支持自定义，您可以通过修改对应的 YAML 文件来：

- 调整颜色方案
- 更换背景图片
- 修改动画效果
- 调整布局参数

## 贡献

我们欢迎各种形式的贡献：

- 提交 Bug 报告
- 提出新功能建议
- 提交代码改进
- 分享主题定制方案

## 许可

MIT License

## 更新日志

### v1.2.0
- 新增新极简主题的三个变体：深蓝、浅绿、深红
- 优化主题切换动画
- 改进移动端适配

### v1.1.0
- 新增智能办公主题
- 优化深色模式显示效果
- 修复已知问题

### v1.0.0
- 首次发布
- 支持6种基础主题
- 实现浅色/深色模式 