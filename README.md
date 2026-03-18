# mxck_interfaces

This package contains all custom ROS2 service and message definitions for the MXCK project.
By keeping interface definitions in a dedicated `ament_cmake` package, we cleanly separate
`.srv` and `.msg` files from Python business logic, allowing any package in the workspace
to import generated types without depending on implementation code.