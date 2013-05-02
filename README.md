Android_Launcher_Custom
=======================

Android_Launcher_Custom
这是Android原生的Launcher(2.3以前的)应用。做了一些修改，让其可以单独进行编译。
修改包括：
1.修改包名，修改包名后安装才不会和系统的冲突 
2.导入编译依赖包。
  1)framework_intermediates/classes.jar (android的框架类)
  2)android-common_intermediates/classes.jar (包含com.android.common.Search这个类)
  3)core_intermediates/classes.jar (包含dalvik.system.VMRuntime这个类)
  这三个包放在根目录的sys_lib文件夹中，编译时将三个包，作为user library引用到项目中来。
