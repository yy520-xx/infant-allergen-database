# 🔍 婴幼儿过敏原数据库 (Infant Allergen Database)

> 常见婴幼儿食品过敏原结构化数据库 —— 配料表关键词、交叉反应、安全替代品，一站查询。

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Allergy](https://img.shields.io/badge/Food-Allergy-red.svg)](#)
[![CMPA](https://img.shields.io/badge/CMPA-Database-blue.svg)](#)

## 📖 项目背景

对于食物过敏宝宝的家长来说，每次买辅食都像在"拆弹"——配料表上密密麻麻的化学名词，到底哪些含牛奶？哪些是隐藏的麸质？哪些是坚果衍生物？

本项目整理了一套结构化的婴幼儿食品过敏原数据库，将常见过敏原的配料表关键词、交叉反应关系和安全替代品汇总成可查询的数据文件，帮助家长快速、准确地判断食品是否安全。

## 🎯 项目目的

- 📊 结构化整理常见婴幼儿食品过敏原数据
- 🏷️ 收录配料表中可能隐藏过敏原的关键词/别名
- 🔄 梳理过敏原之间的交叉反应关系
- ✅ 提供安全替代品推荐
- 🤖 数据采用 JSON 格式，便于程序调用和二次开发

## 📂 项目内容

```
infant-allergen-database/
├── README.md                    # 本文件
├── DISCLAIMER.md                 # 医学免责声明
├── LICENSE                       # MIT 许可证
└── data/                         # 数据目录
    ├── common-allergens.json     # 常见过敏原数据库（结构化JSON）
    ├── ingredient-keywords.md    # 配料表关键词速查表
    ├── cross-reactivity.md       # 过敏原交叉反应图谱
    └── safe-alternatives.md       # 安全替代品推荐
```

## 📋 数据覆盖范围

### 八大主要过敏原
1. 🥛 牛奶（CMPA 重点关注）
2. 🥚 鸡蛋
3. 🌾 小麦/麸质
4. 🫘 大豆
5. 🥜 花生
6. 🌰 坚果
7. 🐟 鱼类
8. 🦐 甲壳类海鲜

### 附加收录
- 芝麻、芥末、芹菜、亚硫酸盐等次级过敏原
- 常见食品添加剂中的过敏原成分
- 加工食品中的隐藏过敏原

## 🚀 使用方式

### 快速查阅
直接浏览 `data/` 目录下的 Markdown 文件，按类别查询。

### 程序调用
`data/common-allergens.json` 为结构化数据，可直接用于开发自己的查询工具或 APP。

```json
{
  "allergen_id": "milk",
  "name_zh": "牛奶",
  "name_en": "Milk",
  "keywords_zh": ["牛奶", "牛乳", "乳清", "酪蛋白", "..."],
  "cross_reactivity": ["羊奶", "马奶"],
  "safe_alternatives": ["深度水解配方", "氨基酸配方", "..."]
}
```

### 自定义扩展
欢迎 Fork 本仓库，补充您所在地区或特殊需求的过敏原数据。

## 🤝 贡献指南

- 发现遗漏的配料表关键词？欢迎提交 PR
- 有新的交叉反应数据？欢迎补充
- 发现错误信息？请提 Issue 指出

## ⚠️ 免责声明

本数据库内容仅供参考，不构成医疗建议。过敏原信息可能因产品配方更新而变化，购买食品时请始终以实际包装配料表为准。详见 [DISCLAIMER.md](DISCLAIMER.md)。

## 📜 License

本项目采用 [MIT License](LICENSE) 开源协议。

## 🔗 相关项目与推荐工具

以下是我们推荐的敏宝育儿相关项目，欢迎一起使用：

### 🌟 主力工具
- **[敏宝喂养工具 (Minbao Feeding Tools)](https://github.com/yy520-xx/minbao-feeding-tools)** —— 面向 CMPA 宝宝的一站式喂养辅助工具集，内置配料表过敏原查询引擎
- **[敏宝育儿资讯站 (Minbao SEO)](https://yy520-xx.github.io/minbao-seo/)** —— 敏宝家庭的育儿知识百科与资源导航

### 📚 相关开源项目
- **[敏宝食谱库 (CMPA Recipe Book)](https://github.com/yy520-xx/cmpa-recipe-book)** —— 专为牛奶蛋白过敏宝宝设计的安全食谱集合
- **[宝宝辅食添加指南 (Baby Solid Food Guide)](https://github.com/yy520-xx/baby-solid-food-guide)** —— 系统化的辅食添加时间表、食材引入顺序与过敏观察指南

---

> 💡 *如果这个项目对你有帮助，欢迎 Star ⭐ 支持我们！*
