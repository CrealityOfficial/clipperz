__tree_add_current(SRCS)
__add_real_target(clipperz lib SOURCE ${SRCS}
							   LIB ${LIBS}
							   INTERFACE ${CMAKE_CURRENT_SOURCE_DIR})
							   
if(CC_INSTALL_CLIPPERZ)
	__install_directory_specif(${CMAKE_CURRENT_SOURCE_DIR}/ clipperz)
endif()