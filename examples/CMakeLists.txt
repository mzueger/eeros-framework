include_directories(${EEROS_SOURCE_DIR}/includes ${EEROS_BINARY_DIR})

add_subdirectory(sequencer)
add_subdirectory(controlSystem)
add_subdirectory(safety)
add_subdirectory(config)

if(LIBCOMEDI)
#	add_subdirectory(simpleMotorController)
endif()

if(LIBFLINK)
#	add_subdirectory(flink)
endif()
