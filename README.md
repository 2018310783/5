# 一、实验目的
1.分析学生选课系统
2.使用GUI窗体及其组件设计窗体界面
3.完成学生选课过程业务逻辑编程
4.基于文件保存并读取数据
5.处理异常
# 二、实验要求
1、设计GUI窗体，支持学生注册、课程新加、学生选课、学生退课、打印学生选课列表等操作。
2、基于事件模型对业务逻辑编程，实现在界面上支持上述操作。
3、针对操作过程中可能会出现的各种异常，做异常处理
4、基于输入/输出编程，支持学生、课程、教师等数据的读写操作。
5、基于Github.com提交实验，包括实验SRC源文件夹程序、README.MD实验报告文档。
# 三、实验过程
1. 分析实验要求，需要运用类之间继承关系。
（1）首先定义五个类，分别是人员people类、教师teachers类、学生students类、课程subject类、测试类SystemTest。
（2）根据要求说明，挖掘其中的逻辑关系；容易发现，通过打印学生信息，可以实现对课程与老师信息的输出，故可以得到他们之间的包含关系：学生信息→课程信息→教师信息，考虑到一个学生只能选一门课，一门课只能由一个老师教授，可知这条单链包含关系就可以使其相关联。
（3）为测试类以外的四个类添加属性与方法，将People类设为Teacher类与Students类的父类，这两个子类可以通过继承获取父类的id、name、sex等属性并且继承相应地方法。
（4）覆盖Object根类中的toString方法，使其可以根据类名返回特定的字符串信息。
2.完善测试类，对多个类进行实例化，调用java.util.Scanner进行交互输入，运用switch语句和条件结构使逻辑更加清晰。
# 四、流程图
