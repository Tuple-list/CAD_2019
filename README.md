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
  + 命令行：  **PLINE(PL)**
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
  > 只有当前文本样式中设置的字符高度为0，在使用**TEXT**命令时，才会出现字符高度提示。允许倾斜角度为30,45，-45时的排列效果。
  > 在“指定文字的旋转角度<0>”提示下输入倾斜角度
+ **多行文本标注**
  + 命令行：  **MTEXT(MT)**  
+ **文本编辑**
  + 命令行：  **DDEDIT(ED)**  
---
**A3模板：420mm*297mm**  
---

### 第四章 精确绘图 
+ **图层**  
  + 命令行：  **LAYER**  
+ **设置线型**  
  + 命令行：  **LINETYPE**  
  + **在线型管理器对话框设置**  
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
  + 极轴追踪：是指按指定的极轴角或极轴角的倍数对齐要指定点的路径；   
  + 对象捕捉追踪：指以捕捉到的特殊位置点为基点，按指定的极轴角或极轴角的倍数对齐要指定点的路径。  
  + 命令行：**DDOSNAP**  
+ **缩放**  
  + 实时缩放 命令行： ZOOM  
  + 操作： 按住鼠标左键垂直向上或向下移动，可以放大或缩小图形  
+ **平移**  
  + 实时平移 命令行： **PAN**  
  + 定点平移 命令行： **-PAN**  
---  
### 第五章  编辑命令  
+ **选择对象**  
  + 方法：  
    ```
    1> 选择编辑命令，然后选择对象，按 **enter** 键结束操作  
    2> 使用 SELECT 命令。在命令行输入“SELECT” ，按enter键，按提示选择对象，按enter键结束    
    3> 利用定点设备选择对象，然后调用编辑命令  
    ```  
  + **部分选项的含义**  
    ```  
    1> 窗口（W）： 用两个对角顶点确定的矩形窗口选择位于其范围内部的所以图形，边界相交的不会选中，指定对角从左向右  
    2> 上一个（L）： 在“选择对象”提示下输入“L”，按<Enter>键，系统自动选择最后绘出的一个图形  
    3> 窗交（C）： 该方法与“窗口”方法类似，其区别在于它不但选中矩形窗口内部的对象，也选中与矩形窗口边界相交的对象  
    4> 框（BOX）： 使用框时，系统根据用户在绘图区指定的两个对角点的位置而自动引用 **窗口** 或 **窗交** 选择方式，若从左向右指定对角点，为“窗口”方式，反之    
    5> 全部（All）： 选择绘图区所有对象  
    6> 栏选（F）： 用户临时绘制一些直线，这些直线不必构成封闭图形，凡是与这些直线相交的对象均被选中  
    7> 圈围（WP）： 使用一个不规则的多边形来选择对象  
    8> 圈交（CP）： 类似于“圈围”方式，输入“CP”，按<Enter>键，后续操作与圈围相同。区别为此操作中 多边形边界相交的对象也被选中  
    ```  
    
+ **复制命令**  
  + 命令行： COPY （CO）   
  + 选项说明：  
    ```
    1> 指定基点： 指定第一个坐标后，该点作为复制对象的基点  
    2> 位移（D）直接输入位移值  
    3> 模式（O）控制是否自动重复该命令，该设置由系统变量控制  
    ```  
+ **镜像命令**  
  + 定义： 选择对象以一条镜像线为轴做对称复制。完成后，可以保留原对象，也可以将其删除   
  + 命令行： **MIRROR(MI)**  
+ **偏移命令**  
  + 命令行：**OFFSET(O)**  
  + 选项说明：  
    ```  
    1> 指定偏移距离：输入距离值，或按Enter键使用当前值，系统把当前值作为偏移的距离  
    2> 通过（T）：指定偏移的通过点  
    3> 删除（E）：偏移原对象后将其删除  
    4> 图层（L）：确定将偏移对象创建在当前图层上还是原对象所在的图层上，这样可以偏移在不同图层上对象。  
    ```  
+ **阵列命令**  
  + 命令行：**ARRAY(AR)**  
  + 选项说明：  
    ```  
    1> “矩形阵列”单选钮： 用于创建矩形阵列，指定参数创建   
    2> “环形阵列”单选钮： 用于创建环形阵列，指定各项参数  
    ```  
+ **移动命令**  
  + 命令行： **MOVE(M)**  
+ **旋转命令**  
  + 命令行： **ROTATE(RO)**  
  + 命令行提示与操作：  
    ```  
    1> 复制（C）：选择此选项，则在旋转对象的同时，保留原对象  
    2> 参照（R）采用参照方式旋转对象  
    ```  
+ **缩放命令**  
  + 命令行：**SCALE(SC)**  
+ **删除命令**  
  + 命令行： **ERASE(E)**  
+ **恢复命令**  
  + 误删图形，可以恢复命令
  + 命令行： **OOPS(U)**  
+ **修剪命令**  
  + 命令行： **TRIM(TR)**  
  + 提示： **在选择对象时，按住Shift键，系统就会自动将“修剪”命令转换成“延伸”命令**
  + 选择“栏选（F）”选项时，系统以栏选的方式选择被“修剪”的对象  
+ **延伸命令**  
  + 命令行：**EXTEND(EX)**  
+ **拉伸命令**  
  + 命令行： **STRETCH(S)**  
+ **拉长命令**  
  + 命令行： **LENGTHEN(LEN)**  
  + 选项说明：  
    1> 增量（DE）: 指定增量方法改变长度，角度  
    2> 百分数（P）： 用指定占总长度百分比的方法改变 **圆弧或直线段的长度**      
    3> 全部（T）：用指定新总长度或总角度值的方法改变对象的 **长度或角度**  
    4> 动态（DY）：在此模式下，可以使用鼠标拖拉的方式来动态地改变对象的 **长度或角度**  
+ **圆角命令**  
  + 命令行： **FILLET (F)**  
  + 选项说明：  
  ```  
    1> 多段线（P）： 在一条二维多线段两段直线段的节点处插入圆弧  
    2> 修剪（T）： 决定在平滑连接两条边时，是否修剪这两条边  
    3> 多个（M）： 同时对多个对象进行圆角编辑，而不必重新起用命令  
    4> 按住<Shift>键并选择两条直线，可以快速创建零距离倒角或零半径圆角  
  ```    
+ **倒角命令**  
  > 倒角命令即斜角命令，是用斜线连接两个不平行的线型对象。  
  + 命令行： **CHAMFER (CHA)**
  + 选项说明：  
  ```  
  1> 多段线（P）：对多段线的各个交叉点倒斜角  
  2> 距离（D）：选择倒角的两个斜线距离。若二者均为 0 ，则不绘制连接，而是把两对象延伸至相交并修剪超出部分  
  3> 角度（A）：选择第一条直线的斜线距离和第一条直线的倒角角度  
  4> 修剪（T）：与圆角连接命令相同，该命令决定连接对象后是否剪切源对象  
  5> 方式（E）：决定采用 ** “距离”方式还是“角度” ** 方式来倒斜角  
  6> 多个（M）：同时对多个对象进行倒斜角编辑  
  ```  
+ **打断命令**  
  + 命令行： **BREAK (BR)**  
  > 打断于点命令： 是指在对象上指定一点，从而把对象在此点拆分成两部分  
+ **分解命令**  
  + 命令行： **EXPLODE (X)**  
  > 该命令选择一个对象后，对象会被分解，系统继续提升该行信息，允许分解多个对象  
  > 分解命令是将一个合成图形分解为其部件的工具。eg： 矩形被分解后变4条直线，且一个有宽度的直线分解后就会失去其宽度属性  
+ **合并命令**  
  + 命令行： **JOIN**  
+ **修改对象属性**  
  + 命令行： **DDMODIYT 或 PROPERTIES**  
---  

### 第六章  表格和尺寸标注  
  
+ **定义表格样式**  
  + 命令行： **TABLESTYLE**  
+ **表格文字编辑**  
  + 命令行： **TABLEDIT**  
+ **尺寸样式**  
  + 命令行： **DIMSTYLE (D)**  
  > 进行尺寸标注前，先创建尺寸标注的样式。如果不创建尺寸样式而直接进行标注，系统使用默认名称为 standard 的样式，部分不合适的再修改。  
+ **标注尺寸**  
  + 命令行： **DIMLINEAR (DLI)**  
  + **对其标注 (DIMALLGNED 快捷命令：DAL)**  
  + **基线标注 (DIMBASELINE 快捷命令：DBA)**  
  + **连续标注 (DIMCONTINUE 快捷命令：DCO)**  
  + **引线标注 (LEADER 快捷命令：LEAD)**  
---  

### 第七章  辅助绘图工具  
  + **定义图块 (BLOCK 快捷命令：B)**  
  + **图块的存盘 (WBLOCK 快捷命令：W)**  
  > 利用 BLOCK 命令定义的图块保存在其所属的图形中，该图块只能在该图中插入，而不能插入到其他的图形中。但有些图块需要在许多图形中经常用的，这时可以用 WBLOCK(W) 命令把图块以图形文件的形式（后缀为.dwg）写入磁盘。图形文件可以在任何图形中用 INSERT(I) 命令插入。  
  + **动态块 (BEDIT 快捷命令：BE)**  
  > 在动态块中，由于属性的位置包括在动作的选择集中，因此必须将其锁定。
  + **图块属性(ATTDEF 快捷命令：ATT)**  
  > 图块除了包含图形对象以外，还可以具有非图形信息，如把一把椅子的图形定义为图块后，还可以把椅子的号码 材料 重量 价格以及说明等文本信息一并加入到图块当中。图块的这些非图形信息，叫做图块的属性，它是图块的一个组成部分，与图形对象一起构成一个整体，在插入图块时会把图形对象连同属性一起插入到图形中。
  + **修改属性定义 (DDEDIT 快捷命令：ED)**  
  > 在定义图块之前，可以对属性的定义加以修改，不仅可以修改属性标签，还可以修改属性提示和属性默认值。  
  + **图块属性编辑 (ATTEDIT 快捷命令：ATE)**  
  > 当属性被定义到图块中，甚至图块被定义到图形当中后，用户还可以对图块属性进行编辑，修改。  
  
