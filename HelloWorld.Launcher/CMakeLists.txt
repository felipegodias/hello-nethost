project(HelloWorld.Launcher CXX)

set(PROJECT_SRC)

add_subdirectory("Src")

list(SORT PROJECT_SRC)
message("\n::::: ${PROJECT_NAME} Source Files Start :::::")
foreach(SRC_FILE IN LISTS PROJECT_SRC)
    message(${SRC_FILE})
endforeach()

add_executable(${PROJECT_NAME} ${PROJECT_SRC})