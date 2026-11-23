---
title: "Skill Scanner — 装技能前先做安全扫描"
source: "https://workbuddy.jiangyufan.com/index/hub/skill/3"
type: "skill"
chars: 416
sections: 4
figures: 0
chapter: "10-我要写代码和做自动化"
---

# Skill Scanner — 装技能前先做安全扫描

> **说明：** 本篇是产品动态/短记录，原文本身只有简短说明和配图，不含完整操作步骤。它被收录是因为记录了当时的界面或功能变化，可作为版本对照；需要完整流程请到对应章节找长文。
## 这是什么
第三方 Skill 本质上是**可执行代码**。Skill Scanner 的核心价值在于：在安装前先对 Skill 做安全审查，帮你发现可疑依赖、硬编码配置和潜在风险，降低误装风险。

## 什么情况用它
- 安装任何第三方 Skill 前先做一次审查。
- 检查是否存在可疑依赖。
- 排查是否有硬编码的私人配置。
- 给新手提供基础安全兜底。

## 怎么用
用于安装技能、包或插件的安全检查。官方特别强调：**在执行任何 npm install、openclaw plugins install、clawhub install 或类似安装命令之前使用。**

## 新手建议
先审计、再安装，这是最推荐的使用顺序。重点关注依赖和脚本，尤其是来源不明的第三方 Skill。适合作为日常安装流程的一部分长期启用。
