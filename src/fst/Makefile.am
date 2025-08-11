## Process this file with automake to produce Makefile.in

## Copyright (C) 2011–2022 Samediggi

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

SUBDIRS = stems

if CAN_HFST_LEXC
check-local:
	$(HFST_LEXC) --Werror -v testroot.lexc \
		stems/arabic_roman_digits.lexc \
		stems/smi-abbreviations.lexc \
		stems/smi-acronyms.lexc \
		stems/smi-digits.lexc \
		stems/smi-propernouns.lexc \
		-o /dev/null
endif

