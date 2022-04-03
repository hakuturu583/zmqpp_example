cmake_minimum_required(VERSION 3.8)
project(zmqpp_example)

add_executable(publish
  publish.cpp
)

target_link_libraries(publish
  zmqpp
  zmq
)

add_executable(subscribe
  subscribe.cpp
)

target_link_libraries(subscribe
  zmqpp
  zmq
)