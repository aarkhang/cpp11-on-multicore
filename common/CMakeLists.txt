cmake_minimum_required(VERSION 3.12)

project(CPP11_OM_Library VERSION 1.0
        LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

add_library(cpp11_om STATIC
    sema.h
    rwlock.h
    inmemorylogger.h
    inmemorylogger.cpp
    diningphilosophers.h
    bitfield.h
    benaphore.h
    autoreseteventcondvar.h
    autoresetevent.h
)
