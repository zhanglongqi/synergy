# synergy -- mouse and keyboard sharing utility
# Copyright (C) 2012 Synergy Si Ltd.
# Copyright (C) 2011 Nick Bolton
# 
# This package is free software; you can redistribute it and/or
# modify it under the terms of the GNU General Public License
# found in the file COPYING that should have accompanied this file.
# 
# This package is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
#
# You should have received a copy of the GNU General Public License
# along with this program.  If not, see <http://www.gnu.org/licenses/>.

add_subdirectory(synergyc)
add_subdirectory(synergys)
add_subdirectory(synergyd)
add_subdirectory(usynergy)
add_subdirectory(syntool)

if (WIN32)
  add_subdirectory(synergyp)
endif()

if (APPLE)
	if (OSX_TARGET_MINOR GREATER 8)
		add_subdirectory(synmacph)
	endif()
endif()
