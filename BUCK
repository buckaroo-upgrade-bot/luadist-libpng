load('//:buckaroo_macros.bzl', 'buckaroo_deps')

cxx_library(
  name = 'png',
  header_namespace = '',
  exported_headers = {
    'png.h': 'png.h',
    'pngconf.h': 'pngconf.h',
    'pnglibconf.h': 'scripts/pnglibconf.h.prebuilt',
  },
  srcs = [
    'png.c',
    'pngerror.c',
    'pngget.c',
    'pngmem.c',
    'pngpread.c',
    'pngread.c',
    'pngrio.c',
    'pngrtran.c',
    'pngrutil.c',
    'pngset.c',
    'pngtrans.c',
    'pngwio.c',
    'pngwrite.c',
    'pngwtran.c',
    'pngwutil.c',
  ],
  visibility = [
    'PUBLIC',
  ],
  reexport_all_header_dependencies = False,
  deps = buckaroo_deps(),
)

cxx_binary(
  name = 'test',
  srcs = [
    'pngtest.c',
  ],
  deps = [
    ':png',
  ],
)
