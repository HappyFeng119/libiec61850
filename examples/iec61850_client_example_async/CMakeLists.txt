
set(iec61850_client_async_SRCS
   client_example_async.c
)

IF(WIN32)
set_source_files_properties(${iec61850_client_async_SRCS}
                                       PROPERTIES LANGUAGE CXX)
ENDIF(WIN32)

add_executable(iec61850_client_async
  ${iec61850_client_async_SRCS}
)

target_link_libraries(iec61850_client_async
    iec61850
)
