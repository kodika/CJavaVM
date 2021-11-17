add_library(CJavaVM
	Sources/CJavaVM/dummy.c
)

target_include_directories(CJavaVM
	INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}/Sources/CJavaVM/include
)

install( DIRECTORY 
	Sources/CJavaVM/include/
	DESTINATION
	lib/swift/CJavaVM
)
