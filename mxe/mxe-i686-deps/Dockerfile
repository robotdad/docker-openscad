#
# Build: docker build -t openscad/mxe-i686-deps .
# Use: docker run --rm -it openscad/mxe-i686-deps
#
FROM openscad/mxe-i686-gcc:latest

WORKDIR /mxe

RUN make JOBS=2 -j2 MXE_PLUGIN_DIRS=plugins/gcc7 MXE_TARGETS=i686-w64-mingw32.static.posix qtbase qtmultimedia qscintilla2 mpfr eigen opencsg cgal nsis glib libxml2 freetype fontconfig harfbuzz libzip
