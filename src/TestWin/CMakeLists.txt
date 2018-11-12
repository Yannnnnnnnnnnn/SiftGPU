find_package(OpenGL REQUIRED)
find_package(GLUT REQUIRED)
find_package(GLEW REQUIRED)

include_directories( ${GLEW_INCLUDE_DIRS} )


ADD_EXECUTABLE(SimpleSIFT SimpleSIFT.cpp)
TARGET_LINK_LIBRARIES(SimpleSIFT dl)


set(CMAKE_VERBOSE_MAKEFILE ON)
