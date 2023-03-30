cmake_minimum_required(VERSION 3.24)
project(QtTest)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)

set(CMAKE_PREFIX_PATH "/Users/lichunxue/Applications/Qt/6.5.0/macos")

find_package(Qt6 COMPONENTS
        Core
        Gui
        Widgets
        REQUIRED)

add_executable(QtTest main.cpp)
target_link_libraries(QtTest
        Qt::Core
        Qt::Gui
        Qt::Widgets
        )

