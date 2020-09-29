# WoodenMan
[![License](https://img.shields.io/badge/Docs-hmsguides-brightgreen)](https://developer.huawei.com/consumer/cn/doc/development/HMS-Guides/ml-introduction-4)

## 目录

 * [介绍](#介绍)
 * [工程目录结构](#工程目录结构)
 * [更多场景](#更多场景)
 * [运行步骤](#运行步骤)
 * [支持的环境](#支持的环境)
 * [许可证](#许可证)


## 介绍
WoodenMan通过HUAWEI ML Kit的人体骨骼检测、图像分割、人脸检测能力，实现了拍一张松山湖游客照，以及根据骨骼点姿势进行闯关的功能。

本demo演示了如何使用[HUAWEI ML Kit] (https://developer.huawei.com/consumer/cn/hms/huawei-mlkit)快速开发人体骨骼检测 图像分割 人脸检测的应用，目的是让您体验人体骨骼检测 图像分割 人脸检测功能，帮助您尽快集成HUAWEI ML Kit。

## 工程目录结构
Smile-Camera

    |-- com.huawei.hms.mlkit.sample
        |-- activity
            |-- ChooserActivity // 入口
            |-- WoodenManActivity // 拍张大会纪念照
            |-- ModelGameStartOneActivity // 摆POSE大闯关

## 更多场景
基于HUAWEI ML Kit提供的 人体骨骼检测 图像分割 人脸检测能力，可以做人像替换背景，还可以实现更加丰富多彩的应用，如：
1、检测人体骨骼检测，通过对比不同造型，实现闯关游戏等。
2、跟踪视频中的人脸、人体骨骼，开发好玩的人脸、骨骼特效。

## 运行步骤
- 准备工作
  - 在项目层build.gradle文件中增加华为Maven仓库。
  - 在应用层build.gradle文件中添加SDK依赖。
  - Android系统manifest.xml中申请相机权限。

- 代码开发的关键步骤
  - 动态权限申请。
  - 创建人体骨骼检测器。
  - 通过android.graphics.bitmap创建用于分析器检测图片的“MLFrame”对象。
  - 调用“createImageTransactor”方法进行图像分割。
  - 调用“createLensEngine”方法初始化人体骨骼检测、人脸检测器。
  - 调用“compareSimilarity”方法实现骨骼相似度对比。

## 支持的环境
推荐使用Android 4.4及以上版本的设备。

##  许可证
此示例代码已获得[Apache 2.0 license]（https://www.apache.org/licenses/LICENSE-2.0）。