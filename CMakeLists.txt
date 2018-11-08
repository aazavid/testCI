# CMakeList.txt: проект CMake для testCI; включите исходный код и определения,
# укажите здесь логику для конкретного проекта.
#
cmake_minimum_required (VERSION 3.8)

project(main)                # Название проекта

set(SOURCE_EXE main.cpp)            # Установка переменной со списком исходников

include_directories(hello)            # Расположение заголовочных файлов

add_executable(main ${SOURCE_EXE})  # Создает исполняемый файл с именем main

add_subdirectory(hello)               # Добавление подпроекта, указывается имя дирректории

target_link_libraries(main hello)     # Линковка программы с библиотекой


