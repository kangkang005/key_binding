# 链接
    http://bbs.eetop.cn/thread-889394-1-1.html
# Cadence 常用快捷
## 鼠标操作
1. 单击左键选中一个图形。如果是两个图形交叠的话,单击左键选中其中一个图形,再单击会选中另一个图形
2. 用左键框选,选中一片图形,图形要被完全包围才会被选中
3. 中键单击调出常用菜单命令
4. 右键点击拖放用来放大。放大后经常配合 F 键使用,恢复到全部显示。配合 Tab 键使用,平移视图。右键还有 “Strokes” ,就是点住右键画些图线,就能实现调用某些命令
5. Shift+ 左键加选图形, Ctrl+ 左键减选图形

## 键盘操作
    F1              显示帮助窗口
    F2              保存
    F3              控制在选取相应工具后是否显示相应属性对话框的。如在选取 Path 工具后,想控制 Path 的走向,可以按 F3 调出对话框进行设置
    F4              Toggle Partial Select ,用来控制是否可以部分选择一个图形
    F5              打开。
    F8              Guided Path Create
    F9              Filter Size
    Ctrl+A          全选
    B               Go to Level
    Shift+B         升到上一级视图
    C               复制。复制某个图形
    Ctrl+C          中断某个命令,不常用。一般多按几次 Esc 键即可取消某个命令
    Shift+C         裁切 (Chop) 。首先调用命令,选中要裁切的图形,后画矩形裁切
    D               取消选择
    Ctrl +D         取消选择。这个也可用鼠标点击空白区域实现
    Shift+D         取消选择
    Shift+E 和 E    控制用户预设的一些选项
    F               满工作区显示。就是显示所有图形
    Ctrl+F          显示上一层级
    Shift+F         显示所有层级
    G               Gravity ,吸附。打开后会吸附到某些节点上
    Ctrl+G          Zoom To Grid
    I               Instance ,插入模块
    K               Ruler ,标尺工具
    Shift+K         清除所有标尺
    L               标签工具。 Label 。标签要加在特定的 text 层上
    M               移动工具。 Move 。点选 Move 工具后,选中要移动的图形,然后在屏幕上任
                    意一处单击一下这个就是确定移动的参考点,然后就可以自由移动了。也可以
                    通过鼠标先选中一个图形,移动鼠标当鼠标箭头变成十字方向的时候就可以拖
                    动来实现。
    Shift+M         Merge ,合并工具
    N               控制走向,斜 45 对角 + 正交
    Ctrl+N          控制走向,先横后竖
    Shift+N         控制走向,直角正交
    O               Create Contact ,插入通孔
    Shift+O         Rotate ,旋转工具
    P               插入 Path
    Ctrl+P          插入引脚( Pin )
    Shift+P         Polygon ,多边形工具
    Q               对象属性
    Shift+Q         打开设计属性对话框
    R               矩形工具
    Ctrl+R          Redraw ,重画
    Shift+R         Reshape 。就是在原来的图形上再补上一块图形
    S               Stretch ,拉伸工具。可以点击图形边框,也可以框选若干图形(边框)再进行拉伸。
    Ctrl+S          Split ,添加拐点。就是配合 Stretch 命令可以将原来直的 Path 打弯
    Shift+S         Search ,查找
    T               Layer Tap ,层切换。使用 T 后再点击一个图形,会自动切换到刚点击图形的
                    层上去。可不必频繁点击 LSW 窗口
    Ctrl+T          Zoom to Set
    Shift+T         Tree
    U               Undo ,撤销
    Shift+U         Redo ,重复
    V               Attatch ,关联。将一个子图形( child )关联到一个父图形( parent )后。关联
                    后,若移动 parent , child 也将跟着移动;移动 child , parent 不会移动。可以
                    将 Label 关联到 Pad 上
    Ctrl+V          Type in CIW
    W               Previous View ,前一视图
    Ctrl+W          关闭窗口
    Shift+W         Next View ,下一个视图
    X               Edit in Place
    Ctrl+X          Fit Edit
    Shift+X         Descend ,下降一等级
    Y               Yank ,区域复制。和 Copy 是有区别的, Copy 只能复制完整图形对象
    Ctrl+Y          Cycle Select
    Shift+Y         Paste ,粘贴。配合 Yank 使用
    Z               视图放大
    Ctrl+Z          Zoom In by 2 ,视图放大两倍
    Shift+Z         Zoom Out by 2 ,视图缩小两倍
    ESC             Cancel
    Tab             平移视图 Pan 。按 Tab ,用鼠标点击视图区中某点,视图就会移至以该点为中心
    Delete          删除
    BackSpace       撤销上一点。在 Path 一点画错时,可以撤销上一点
    Enter           确定一个图形的最后一点。也可双击鼠标左键结束
    Ctrl+ 方向键    移动 Cell
    Shift+ 方向键   移动鼠标。每次半个格点的距离
    方向键          移动视图
