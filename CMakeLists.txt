cmake_minimum_required(VERSION 3.31)
project(Encryptor)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)

set(CMAKE_PREFIX_PATH "/Volumes/Crucial/QT/6.10.0/macos/bin")

find_package(Qt6 COMPONENTS
        Core
        Gui
        Widgets
        REQUIRED)

add_executable(Encryptor main.cpp)
target_link_libraries(Encryptor
        Qt::Core
        Qt::Gui
        Qt::Widgets
)

