add_library(nmea0183_manager SHARED f_nmea0183_manager.cpp ${CHANS})

target_include_directories(nmea0183_manager PUBLIC ${PROJECT_SOURCE_DIR}/include)
target_include_directories(nmea0183_manager PUBLIC ${PROJECT_SOURCE_DIR}/channels)

install(TARGETS nmea0183_manager DESTINATION lib)
