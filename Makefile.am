
AUX_DIST_GEN = $(ac_aux_dir)

EXTRA_DIST = $(AUX_DIST_GEN) libcalg-1.0.pc.in STYLE.md
MAINTAINERCLEANFILES = $(AUX_DIST_GEN)

pkgconfigdir = $(libdir)/pkgconfig
pkgconfig_DATA = libcalg-1.0.pc

$(pkgconfig_DATA) : config.status

SUBDIRS=src test doc

format:
	clang-format -i */*.[ch]
