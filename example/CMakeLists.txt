
PROJECT(example)

ADD_EXECUTABLE(rewrite
rewrite.cxx)

TARGET_LINK_LIBRARIES(rewrite
Cifti
Nifti
Common
${QT_LIBRARIES}
${LIBS})

ADD_EXECUTABLE(xmlinfo
xmlinfo.cxx)

TARGET_LINK_LIBRARIES(xmlinfo
Cifti
Nifti
Common
${QT_LIBRARIES}
${LIBS})

INCLUDE_DIRECTORIES(
${CMAKE_SOURCE_DIR}/example
${CMAKE_SOURCE_DIR}/Common
${CMAKE_SOURCE_DIR}/Nifti
${CMAKE_SOURCE_DIR}/Cifti
)
