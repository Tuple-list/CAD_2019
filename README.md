# CAD_2019
## 操作命令总结  
---
---
### 第三章 二维绘图命令
+ **直线段**  
  + 命令行：**LINE（L）**
  + 正交模式只能绘制水平垂直方向
  
+ **构造线**  
  + 命令行：**XLINE（XL）**  
  + 构造线模拟作图的辅助作图线  
+ **圆形**  
  + 命令行：  **CIRCLE（C）** 

+ **圆弧**  
  + 命令行  
  + ARC(A)
  + 注意：圆弧的曲率是遵循逆时针方向  
+ **圆环**  
  + 命令行：  **DONUT(DO)**
  + 若指定内直径为0，画出实心填充园  
  + 用FILL可以控制圆环是否填充  
+ **椭圆与椭圆弧**  
  + 命令行：  **ELLIPSE**  
+ **矩形**  
  + 命令行：  **RECTANG(REC)**  
+ **正多边形**  
  + 命令行：  **POLYGON(POL)**
+ **图案填充**  
  + 命令行：  **BHATCH(H)**
+ **编辑填充的图案**  
  + 命令行：  **HATCHEDIT(HE)**  
+ **多段线**
  + 命令行  
  + **PLINE(PL)**
+ **样条曲线**
  + 命令行：  **SPLINE(SPL)**
+ **多线**
  + 命令行：  **MLINE(ML)**
  + **定义多线样式**
    命令行：**MLSTYLE**
+ **文本样式**
  + 命令行：  **STYLE(ST)或DDSTYLE**
+ **文本标注**
  + 命令行：  **TEXT(SPL)**  
  + 只有当前文本样式中设置的字符高度为0，在使用**TEXT**命令时，才会出现字符高度提示。允许倾斜角度为30,45，-45时的排列效果。
  + 在“指定文字的旋转角度<0>”提示下输入倾斜角度
+ **多行文本标注**
  + 命令行：  **MTEXT(MT)**  
+ **文本编辑**
  + 命令行：  **DDEDIT(ED)**  
---
**A3模板：420mm*297mm**  
---

### 第四章  
+ **图层**  
  + 命令行：  **LAYER**  
+ **设置线型**  
  + 命令行：  **LINETYPE**  
  + **在线型管理器对话框设置**  
---
+ **正交模式**  
  + 命令行： **ORTHO**  
  + 绘制水平/垂直直线  
+ **对象捕捉**  
  + 识别特殊点的工具  
  + 快捷命令： **MID：中点， CEN： 圆心， EXT：延长线， PAR：平行线**  
  + 捕捉设置：  **DDOSNAP**  
+ **对象追踪**  
  + 定义：是指按指定角度或与其他对象建立指定关系绘制对象  
  + 自动追踪： 包括“极轴追踪”和“对象捕捉追踪”  
  > 极轴追踪：是指按指定的极轴角或极轴角的倍数对齐要指定点的路径；   
  > 对象捕捉追踪：指以捕捉到的特殊位置点为基点，按指定的极轴角或极轴角的倍数对齐要指定点的路径。  
  + 命令行：**DDOSNAP**  
+ **缩放**  
  + 命令行： ZOOM  
  + 操作



