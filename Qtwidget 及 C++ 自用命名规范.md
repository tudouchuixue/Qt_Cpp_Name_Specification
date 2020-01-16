# Qtwidget 及 C++ 自用命名规范

标签（空格分隔）： Qt&C++

---

#文件
文件全部小写
尽量与类名一致
如需分隔使用下划线“_”
例如：
*myusefulclass.cc*
*myuseful_class.cc*

#类
##普通类
驼峰命名 不含下划线
例如：
*MyClass*
*MySuperClass*

##弹出窗口类
驼峰命名 不含下划线 以 Dialog 或 Window 结尾
例如：
*MyClassDialog*
*MySuperClassWindow*

#结构体
特殊的类 在尾加_T
*FieldBuffer_T*
*PackageParameter_T

#函数
##普通函数
首字母为动词，小写
之后符合驼峰命名法
例如：
*openSerialPort*
*clearDataImformation*

##槽函数
槽函数本质上为函数，在最后添加一条下划线代表槽函数。
例如：
*openSerialPort_*

#变量
##普通变量
全为小写，以下划线连接单词，函数参数也归为变量类型
变量先说是什么，再说有什么用
例如：
*data_save_temp*
*dlg_control_img*

##成员变量
类的成员变量本质为变量，或者叫做属性，满足变量命名规则。
增加以下划线“_”结尾的要求。
例如：
*dlg_control_img_*

##widget 控件变量
widget 控件本质上为变量，故命名时仍应遵守变量命名规则。
命名时用小写字母，通过下划线 “_” 间隔，最后以 “控件名” + 下划线 “_” 结尾。如 aaa_bbb_combobox_，ccc_ddd_button_。

#常量
##普通 const 常量
const变量，或在程序运行期间其值始终保持不变的, 命名时以小写“k” 开头,之后采用驼峰命名法。
例如：
*const int kSendData = 100;*

##宏
全部大写。
例如：
*#define ROUND(x) ...*
*#define PI_ROUNDED 3.0*





