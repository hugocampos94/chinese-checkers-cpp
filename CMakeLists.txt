cmake_minimum_required(VERSION 3.10)

project(chinese-checkers-cpp)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

include_directories(include)

add_executable(chinese-checkers-cpp
  src/Game.cpp
  src/Coordinate.cpp
  src/Board.cpp
  src/Movement.cpp
  src/Player.cpp
  src/PlayerPositions.cpp
  include/Game.h
  include/Coordinate.h
  include/Board.h
  include/Movement.h
  include/Player.h
  include/PlayerPositions.h
)