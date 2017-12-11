lib_LTLIBRARIES = libxash.la libxashds.la

BASE_CFLAGS = -lm -ldl -lpthread
BASE_SOURCES = \
    common/avikit.c \
    common/base_cmd.c \
    common/build.c \
    common/cfgscript.c \
    common/cmd.c \
    common/common.c \
    common/con_utils.c \
    common/crashhandler.c \
    common/crclib.c \
    common/crtlib.c \
    common/cvar.c \
    common/dedicated.c \
    common/filesystem.c \
    common/host.c \
    common/hpak.c \
    common/identification.c \
    common/infostring.c \
    common/launcher.c \
    common/library.c \
    common/mathlib.c \
    common/matrixlib.c \
    common/model.c \
    common/mod_studio.c \
    common/net_buffer.c \
    common/net_chan.c \
    common/net_encode.c \
    common/net_huff.c \
    common/network.c \
    common/pm_surface.c \
    common/pm_trace.c \
    common/random.c \
    common/Sequence.c \
    common/sys_con.c \
    common/system.c \
    common/titles.c \
    common/world.c \
    common/zone.c \
    \
    common/imagelib/img_bmp.c \
    common/imagelib/img_dds.c \
    common/imagelib/img_main.c \
    common/imagelib/img_quant.c \
    common/imagelib/img_tga.c \
    common/imagelib/img_utils.c \
    common/imagelib/img_wad.c \
    \
    common/soundlib/libmpg/common.c \
    common/soundlib/libmpg/dct64_i386.c \
    common/soundlib/libmpg/decode_i386.c \
    common/soundlib/libmpg/interface.c \
    common/soundlib/libmpg/layer2.c \
    common/soundlib/libmpg/layer3.c \
    common/soundlib/libmpg/tabinit.c \
    \
    common/soundlib/snd_main.c \
    common/soundlib/snd_mp3.c \
    common/soundlib/snd_utils.c \
    common/soundlib/snd_wav.c \
    \
    server/sv_client.c \
    server/sv_cmds.c \
    server/sv_custom.c \
    server/sv_filter.c \
    server/sv_frame.c \
    server/sv_game.c \
    server/sv_init.c \
    server/sv_log.c \
    server/sv_main.c \
    server/sv_move.c \
    server/sv_phys.c \
    server/sv_pmove.c \
    server/sv_save.c \
    server/sv_world.c


libxash_la_LIBADD = $(BASE_CFLAGS) $(SDL2_LIBS)
libxash_la_CFLAGS = -I common -I ../common -I ../pm_shared -I client -I server -I client/vgui \
    $(SDL2_CFLAGS) \
    -DXASH_SDL

libxash_la_SOURCES = \
    $(BASE_SOURCES) \
    platform/sdl/events.c \
    platform/sdl/gl_sdl.c \
    platform/sdl/gl_sdl_static.c \
    platform/sdl/snd_sdl.c \
    platform/sdl/vid_sdl.c \
    \
    client/cl_cmds.c \
    client/cl_demo.c \
    client/cl_events.c \
    client/cl_frame.c \
    client/cl_game.c \
    client/cl_main.c \
    client/cl_menu.c \
    client/cl_mobile.c \
    client/cl_netgraph.c \
    client/cl_parse.c \
    client/cl_pmove.c \
    client/cl_remap.c \
    client/cl_scrn.c \
    client/cl_tent.c \
    client/cl_video.c \
    client/cl_view.c \
    client/console.c \
    client/gamma.c \
    client/gl_backend.c \
    client/gl_beams.c \
    client/gl_cull.c \
    client/gl_decals.c \
    client/gl_draw.c \
    client/gl_image.c \
    client/gl_mirror.c \
    client/gl_refrag.c \
    client/gl_rlight.c \
    client/gl_rmain.c \
    client/gl_rmath.c \
    client/gl_rmisc.c \
    client/gl_rpart.c \
    client/gl_rsurf.c \
    client/gl_sprite.c \
    client/gl_studio.c \
    client/gl_warp.c \
    client/input.c \
    client/input_evdevkey.c \
    client/joyinput.c \
    client/keys.c \
    client/s_dsp.c \
    client/s_load.c \
    client/s_main.c \
    client/s_mix.c \
    client/s_mouth.c \
    client/s_stream.c \
    client/s_stub.c \
    client/s_utils.c \
    client/s_vox.c \
    client/touch.c \
    client/vid_common.c \
    \
    client/vgui/vgui_draw.c

libxashds_la_LIBADD = $(BASE_CFLAGS)
libxashds_la_CFLAGS = -I common -I ../common -I ../pm_shared -I client -I server -I client/vgui \
    -DXASH_DEDICATED
libxashds_la_SOURCES = \
    $(BASE_SOURCES)