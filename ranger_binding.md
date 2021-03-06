# 1 安装
    sudo apt-get install ranger
官方网站: http://ranger.nongnu.org/

# 2 配置
## 2.1 配置文件
首先复制配置文件到主目录:
    ranger --copy-config=all
然后自己到~/.config/ranger中配置各种选项即可.

## 2.2 配置ranger
在～/.config/ranger中有ranger的配置文件.
找到文件scope.sh中, 在externsions部分注释掉不想预览的文件类型, 在那行上面添加"#"注释掉即可. ranger在预览rar等压缩包时会运行得比较慢.
rc.conf保存着快捷键的说明

## 2.3 自动挂载U盘等外部存储位置,需要安装usbmount:
    sudo apt-get install usbmount
    sudo vim /etc/usbmount/usbmount.conf
在MOUNTOPTIONS那行添加user即可使普通用户也对挂载的U盘拥有写权限, 如下: MOUNTOPTIOS="rw,user,noatime,nodiratime"

# 3 Ranger常用快捷键
    ?  查看帮助

##  浏览(scan):
    H   后退
    L   前进
    gg  跳到顶端
    G   跳到底端
    gh  go home
    gn  新建标签
    f   查找
    /   搜素
    g   快速进入目录

## 编辑(edit):
    space   选择
    uv      取消选择
    yy      复制
    dd      剪切
    pp      粘贴
    delete  删除
    cw      重命名
    A       在当前名称基础上重命名
    I       类似A, 但是光标会跳到起始位置
    Ctrl-f  向下翻页
    Ctrl-b  向上翻页

## 书签(mark):
    m       新建书签
    `       打开书签
    um      删除书签

## 标签(tag):
    gn / C-n        新建标签
    TAB / S-TAB     切换标签
    A-Right, A-Left 切换标签
    gc / C-w        关闭标签

## 排序(order):
    on/ob   根据文件名进行排序(natural/basename)
    oc      根据改变时间进行排序 (Change Time 文件的权限组别和文件自身数据被修改的时间)
    os      根据文件大小进行排序(Size)
    ot      根据后缀名进行排序 (Type)
    oa      根据访问时间进行排序 (Access Time 访问文件自身数据的时间)
    om      根据修改进行排序 (Modify time 文件自身内容被修改的时间)

## 其他(miscellanous):
    zh      显示隐藏文件
    zp      打开/关闭文件预览功能
    zP      打开目录预览功能

## 链接(Link):
    pl      粘贴绝对路径的链接
    pL      粘贴相对路径的链接
    phl     硬链接

## 批量改名(batch edit):
    批量选择文件后, 键入命令:bulkname, 会打开编辑器, 其中的文件名编辑后保存退出, 再次打开操作确认编辑, 然后就批量改名了, 如果想取消批量改名, 在确认时把文件内容删除即可.

## 任务管理(job manager):
    在执行某些操作(比如复制一个大文件)时不能立即完成, 这在 ranger 中就是一个任务. 你可以停止, 启动某个任务, 也可以对某个任务设置优先级.
    w: 打开/关闭任务视图. 在w打开的任务视图中:
        dd: 终止一个任务
        J: 降低当前任务的优先级
        K: 提升当前任务的优先级

## 其他(miscellanous):
    zf      过滤器(如过滤pdf文件, zf+pdf,回车)
    S       在当前目录打开终端
    z(*)    改变设置, *表示在弹出选项中的选择
    o(*)    改变排序方式
    ! / s   使用shell命令(！shell -w ls -hl %s,%s代表当前被选中的文件)
    :       使用ranger命令(3? 查看可用命令)
    :set colorscheme snow 设置颜色模式

# 4 快速预览
安装一下程序可以实现快速预览:
    elinks, html
    highlight,text/code
    img2txt,image
    atool,压缩包
    pdf2text,pdf
    medinfo,audio/video
