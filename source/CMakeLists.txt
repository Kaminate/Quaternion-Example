add_subdirectory(stb)
add_subdirectory(imgui)
IF (WIN32)
	add_subdirectory(windows)
ELSE()
  message( FATAL_ERROR "Unhandled platform" )
ENDIF()

