# Gmsh - Copyright (C) 1997-2016 C. Geuzaine, J.-F. Remacle
#
# See the LICENSE.txt file for license information. Please report all
# bugs and problems to the public mailing list <gmsh@onelab.info>.

set(SRC
  zip.c
  unzip.c
  ioapi.c
  zipper.cpp
  unzipper.cpp
)

file(GLOB_RECURSE HDR RELATIVE ${CMAKE_CURRENT_SOURCE_DIR} *.h)
append_gmsh_src(contrib/zipper "${SRC};${HDR}")
