cmake_minimum_required(VERSION 2.8.9)

project(LinearRegistration)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "http://wiki.slicer.org/slicerWiki/index.php/Documentation/Nightly/Modules/LinearRegistration")
set(EXTENSION_CATEGORY "Legacy.Registration")
set(EXTENSION_CONTRIBUTORS "Daniel Blezek (GE)")
set(EXTENSION_DESCRIPTION "Registers two images together using a rigid transform and mutual information.")
set(EXTENSION_ICONURL "")
set(EXTENSION_SCREENSHOTURLS "")

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(LinearRegistration)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_CPACK})
