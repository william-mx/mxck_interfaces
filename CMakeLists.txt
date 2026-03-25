cmake_minimum_required(VERSION 3.5)
project(mxck_interfaces)

find_package(ament_cmake REQUIRED)
find_package(ament_cmake_python REQUIRED)
find_package(rosidl_default_generators REQUIRED)

rosidl_generate_interfaces(${PROJECT_NAME}
  "srv/SetMode.srv"
)

ament_python_install_package(mxck_interfaces_py)

ament_export_dependencies(rosidl_default_runtime)
ament_package()