CMAKE_MINIMUM_REQUIRED (VERSION 2.6)
PROJECT( asmlib-opencv )
FIND_PACKAGE( OpenCV REQUIRED )
SET(LIB_SRC_LIST feature_extracter_normline_noscaling.cpp featureextracter.cpp modelfile.cpp asmmodel.cpp shapevec.cpp similaritytrans.cpp afreader.cpp modelimage.cpp  shapemodel.cpp shapeinfo.cpp)

INCLUDE_DIRECTORIES( ${OpenCV_INCLUDE_DIRS} )

ADD_LIBRARY( asm STATIC ${LIB_SRC_LIST} )

