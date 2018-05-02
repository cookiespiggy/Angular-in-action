# 第一个Angular项目
1. ng new taskmgr --skip-install --style=scss  新建项目 跳过安装 用scss的形式编写css
2. sudo cnpm install 安装
3. ng g m core 新建一个核心模块
4. ng g m shared 新建共享模块
5. 如何实现让core模块仅加载一次
   思路:
    CoreModule既然是一个类,那么就有构造函数,在构造函数中进行依赖注入CoreModule
6. 作为共享模块,我们要导入模块再导出
7. 在app模块导入一次CoreModule
8. ng g c core/header --spec=false
9. ng g c core/footer --spec=false
10. ng g c core/sidebar --spec=false
11. 编写主html布局
12. 在CoreModule导出三个component
13. ng server 启动工程
