This projects contains the source code for an LPC1114 (Cortex-M0) based hardware board with DOGS102 display and GPS module.

# Download #
[gps\_tracker.hex](https://arm-gps-tracker.googlecode.com/hg/bin/gps_tracker.hex)

# Software Components #
This project contains code from several sources:
  * GLCD library U8glib http://code.google.com/p/u8glib/, License: [New BSD License](http://opensource.org/licenses/BSD-3-Clause)
  * U8glib font licenses are here: http://code.google.com/p/u8glib/wiki/fontgroupx11, http://code.google.com/p/u8glib/wiki/fontgroupadobex11
  * User Interface Library M2tklib http://code.google.com/p/m2tklib/, License [GNU GPL v3](http://www.gnu.org/licenses/gpl.html)
  * LPC1114 specific code (CMSIS) are downloaded from http://www.nxp.com/products/microcontrollers/cortex_m0_m0/LPC1114FN28.html (see application notes). See https://code.google.com/p/arm-gps-tracker/source/browse/src/system_LPC11xx.h as an example for license information.
# Build and Upload Instruction #
## Preconditions ##
  * Download and install the arm gcc from https://launchpad.net/gcc-arm-embedded/. This firmware has been tested with gcc-arm-none-eabi-4\_7-2013q2.
  * Download and install lpc21isp from http://sourceforge.net/projects/lpc21isp/.
  * Clone the hg repository from this project.
## Build and Upload ##
  * If required, update pathnames to the arm gcc and lpc21isp in src/Makefile.
  * Inside the "src" directory of the repository, type "make upload".

