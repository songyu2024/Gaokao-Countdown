# 高考倒计时 - 液体玻璃效果版

一个基于Web的高考倒计时应用，采用现代液体玻璃（Liquid Glass）视觉效果设计。

## ✨ 特性

- 🎓 **精准倒计时**：实时显示距离高考的剩余时间（天、时、分、秒）
- 🌟 **液体玻璃效果**：采用先进的CSS滤镜和背景模糊技术，呈现类似macOS的液体玻璃质感
- 🌤️ **天气显示**：集成天气信息显示
- 💬 **每日一言**：随机显示励志语句，为备考加油
- 📱 **响应式设计**：完美适配桌面端和移动端设备
- 🎨 **自定义背景**：支持自定义背景图片

## 🖼️ 效果预览

应用采用三层卡片式布局：
- **天气卡片**：显示当前天气状况和温度
- **倒计时卡片**：显示高考倒计时的核心信息
- **一言卡片**：显示励志名言或诗句

所有卡片都采用液体玻璃效果，具有：
- 背景模糊（backdrop-filter）
- 玻璃扭曲效果（SVG滤镜）
- 光泽反射效果
- 悬停动画交互

## 🚀 快速开始

### 本地运行

1. 克隆项目到本地
```bash
git clone [your-repo-url]
cd gaokao-countdown-lq_glass
```

2. 准备背景图片
   - 将背景图片命名为 `bg.jpg`
   - 放置在 `img/` 文件夹中

3. 准备字体文件（可选）
   - 将字体文件放置在 `front/` 文件夹中
   - `AaLanTingTiShi-LuoBiRuShen-2.ttf`：用于中文显示
   - `DS-DIGI-1.ttf`：用于数字显示

4. 使用本地服务器运行
```bash
# 使用Python
python -m http.server 8000

# 或使用Node.js的http-server
npx http-server

# 或直接用浏览器打开index.html（某些功能可能受限）
```

5. 在浏览器中访问 `http://localhost:8000`

## 📁 项目结构

```
gaokao-countdown-lq_glass/
├── index.html          # 主页面
├── style.css           # 样式文件
├── script.js           # JavaScript逻辑
├── img/
│   └── bg.jpg          # 背景图片
├── front/
│   ├── AaLanTingTiShi-LuoBiRuShen-2.ttf  # 中文字体
│   └── DS-DIGI-1.ttf   # 数字字体
└── README.md
```

## 🛠️ 技术栈

- **HTML5**：页面结构
- **CSS3**：样式和液体玻璃效果
  - CSS滤镜（backdrop-filter）
  - SVG滤镜效果
  - CSS动画和过渡
- **JavaScript**：倒计时逻辑和API调用
- **SVG**：玻璃扭曲效果滤镜

## ⚙️ 自定义配置

### 修改高考日期
在 `script.js` 中找到并修改目标日期：
```javascript
const examDate = new Date('2024-06-07 09:00:00'); // 修改为目标高考日期
```

### 更换背景图片
替换 `img/bg.jpg` 文件，建议使用高分辨率图片以获得最佳效果。

### 调整液体玻璃效果
在 `style.css` 中可以调整以下参数：
- `backdrop-filter: blur(3px)`：背景模糊程度
- `background: rgba(255, 255, 255, 0.25)`：玻璃透明度
- SVG滤镜参数：扭曲和光照效果

## 🌐 浏览器兼容性

- ✅ Chrome 76+
- ✅ Firefox 103+
- ✅ Safari 14+
- ✅ Edge 79+

**注意**：液体玻璃效果需要现代浏览器支持，旧版浏览器可能显示为普通半透明效果。

## 📝 许可证

本项目采用 MIT 许可证 - 详见 [LICENSE](LICENSE) 文件

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

## 📞 联系方式

如有问题或建议，请通过以下方式联系：
- 提交 GitHub Issue
- [你的联系方式]

---

**为所有高考学子加油！愿你们都能考出理想的成绩！** 🎓✨
