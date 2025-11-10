cmake_minimum_required(VERSION 3.4.1)

add_library(p7zip_jni SHARED
    p7zip_jni.cpp
)

find_library(log-lib
             log)

add_subdirectory(p7zip-17.05)

target_link_libraries(p7zip_jni
                      p7zip
                      ${log-lib})
