## Process this file with autoconf to produce configure script

## Copyright (C) 2011-2022 Samediggi

## This program is free software: you can redistribute it and/or modify
## it under the terms of the GNU General Public License as published by
## the Free Software Foundation, either version 3 of the License, or
## (at your option) any later version.

## This program is distributed in the hope that it will be useful,
## but WITHOUT ANY WARRANTY; without even the implied warranty of
## MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
## GNU General Public License for more details.

## You should have received a copy of the GNU General Public License
## along with this program.  If not, see <http://www.gnu.org/licenses/>.
AC_INIT([shared-smi], [0.0.1], [bugs@divvun.no], [shared-smi], [http://divvun.no])
AC_CONFIG_AUX_DIR([build-aux])
AM_INIT_AUTOMAKE([1.9 tar-pax -Wall -Werror foreign])

## Program checks:
AC_PROG_MKDIR_P()
AC_PROG_INSTALL()

# for checks
AC_PATH_PROG([HFST_LEXC], [hfst-lexc], false)
AM_CONDITIONAL([CAN_HFST_LEXC], [test x$HFST_LEXC != xfalse])
AC_CONFIG_FILES([Makefile src/Makefile src/fst/Makefile src/fst/stems/Makefile \
                 src/cg3/Makefile $PACKAGE.pc])
AC_OUTPUT

cat<<EOF
-- Building $PACKAGE_STRING:

Running make here will probably do nothing... make install may install the
sources but they can just as easily be used in place so it is not necessary at
the moment.
EOF
