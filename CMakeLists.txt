file(GLOB ZIPLIBEXT_SRCS
    ${CMAKE_CURRENT_SOURCE_DIR}/Source/ZipLib/extlibs/zlib/*.c
    ${CMAKE_CURRENT_SOURCE_DIR}/Source/ZipLib/extlibs/lzma/unix/*.c
    ${CMAKE_CURRENT_SOURCE_DIR}/Source/ZipLib/extlibs/bzip2/*.c
)

file(GLOB ZIPLIBDETAIL_SRCS
    ${CMAKE_CURRENT_SOURCE_DIR}/Source/ZipLib/detail/*.cpp
)

file (GLOB ZIPLIB_SRCS
    ${CMAKE_CURRENT_SOURCE_DIR}/Source/ZipLib/*.cpp
)

set(SRC_LIST
   ${SRC_LIST}
   ${ZIPLIB_SRCS}
   ${ZIPLIBEXT_SRCS}
   ${ZIPLIBDETAIL_SRCS}
  
   PARENT_SCOPE
)
