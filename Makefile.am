# 
#  Copyright 2005  Red Hat, Inc.
# 
#  Permission to use, copy, modify, distribute, and sell this software and its
#  documentation for any purpose is hereby granted without fee, provided that
#  the above copyright notice appear in all copies and that both that
#  copyright notice and this permission notice appear in supporting
#  documentation, and that the name of Red Hat not be used in
#  advertising or publicity pertaining to distribution of the software without
#  specific, written prior permission.  Red Hat makes no
#  representations about the suitability of this software for any purpose.  It
#  is provided "as is" without express or implied warranty.
# 
#  RED HAT DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE,
#  INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS, IN NO
#  EVENT SHALL RED HAT BE LIABLE FOR ANY SPECIAL, INDIRECT OR
#  CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
#  DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER
#  TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
#  PERFORMANCE OF THIS SOFTWARE.

bin_PROGRAMS = fonttosfnt

fonttosfnt_CFLAGS = $(FONTTOSFNT_CFLAGS) -DXVENDORNAME=\"X.org\ Foundation\" -DXVENDORNAMESHORT=\"X.org\" -D_BSD_SOURCE
fonttosfnt_LDADD = $(FONTTOSFNT_LIBS) -lm

fonttosfnt_SOURCES =	\
        fonttosfnt.c \
        fonttosfnt.h \
        read.c \
        struct.c \
        util.c \
        write.c

if NEED_SETENV
fonttosfnt_SOURCES += env.c
fonttosfnt_CFLAGS += -DNEED_SETENV
endif

dist_man1_MANS = \
        fonttosfnt.man

