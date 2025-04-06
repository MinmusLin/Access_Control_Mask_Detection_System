# Access Control Mask Detection System

## 项目名称

Access_Control_Mask_Detection_System

## 项目简介

Access control mask detection system.

门禁检测口罩佩戴系统。

> ***Relevant project***
> * 同济大学2023年大学生创新创业训练计划项目

## 项目组成

* [Dataset](Dataset)
数据集

* [Results](Results)
模型训练结果

* [Project Plan Application](20230302_Project_Plan_Application.pdf)
项目计划申请书

* [Opening Defense](20230325_Opening_Defense.pptx)
项目开题答辩

* [First Quarter Report](20230710_First_Quarter_Report.pdf)
项目第一季度报告

* [Second Quarter Report](20231013_Second_Quarter_Report.pdf)
项目第二季度报告

* [Mid-term Defense](20231105_Mid-term_Defense.pptx)
项目中期答辩

* [Mid-term Report](20231105_Mid-term_Report.pdf)
项目中期检查报告

* [Third Quarter Report](20240122_Third_Quarter_Report.pdf)
项目第三季度报告

* [Fourth Quarter Report](20240301_Fourth_Quarter_Report.pdf)
项目第四季度报告

* [Final Report](20240315_Final_Report.pdf)
项目结题报告

* [Final Defense](20240322_Final_Defense.pptx)
项目结题答辩

* [Certificate](Certificate.pdf)
校级大学生创新创业训练计划结题证书

## 模型训练与检测代码

* 模型训练代码

  ```python
  from ultralytics import YOLO

  model = YOLO('yolov8n.pt')
  model.train(data='Dataset/data.yaml', workers=0, epochs=100, batch=16)
  ```

* 模型检测代码

  ```python
  from ultralytics import YOLO

  yolo = YOLO('Train/weights/best.pt', 'detect')
  result = yolo(source=0, show=True)
  ```

## 文档更新日期

2025年3月21日
