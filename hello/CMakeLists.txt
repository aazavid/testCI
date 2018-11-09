cmake_minimum_required (VERSION 2.8)


project(hello)                # Название проекта

set(SOURCE_LIB hello.cpp)     # Установка переменной со списком исходников

add_library(hello STATIC ${SOURCE_LIB})# Создание статической библиотеки




