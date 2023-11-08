# 配置动态库
add_library(func_shared SHARED func.cpp)
# 重命名
set_target_properties(func_shared PROPERTIES OUTPUT_NAME "func")
# 设置版本号
set_target_properties(func_shared PROPERTIES VERSION 1.0 SOVERSION 1)

# 配置静态库
add_library(func_static STATIC func.cpp)
# 重命名
set_target_properties(func_static PROPERTIES OUTPUT_NAME "func")
# 设置版本号
set_target_properties(func_static PROPERTIES VERSION 1.0 SOVERSION 1)