bin_PROGRAMS = xash3d xashds

xash3d_SOURCES = xash.c
xash3d_CFLAGS = $(SDL2_CFLAGS)
xash3d_LDADD = -ldl $(SDL2_LIBS)

xashds_SOURCES = xash.c
xashds_CFLAGS = -DXASH_DEDICATED
xashds_LDADD = -ldl