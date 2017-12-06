#声明要求的cmake的最低版本
cmake_minimum_required( VERSION 2.8 )

#声明一个cmake工程
project(helloSLAM)

#添加一个可执行程序
#语法: add_executable( 程序名 源代码文件 )
add_executable( helloSLAM helloSLAM.cpp )

#把libHelloSLAM.cpp文件编译成一个叫hello的库
#add_library( hello libHelloSLAM.cpp ) 

#生成一个共享库，省空间，得到.so后缀的文件
add_library( hello_shared SHARED libHelloSLAM.cpp)

#添加一个可执行程序，并链接到使用的库上
add_executable( useHello useHello.cpp )
target_link_libraries( useHello hello_shared )
