test_cds_CFLAGS = -m64 -DLINUX_CLIENT -D_FILE_OFFSET_BITS=64 -D_LARGEFILE64_SOURCE -I$(top_srcdir)/src/lib -I@TSM_SRC_DIR@/ -I@LUSTRE_SRC_DIR@/lustre/include

noinst_HEADERS = CuTest.h test_utils.h
bin_PROGRAMS = test_cds
test_cds_SOURCES = test_cds.c CuTest.c test_dsstruct64_off64_t.c test_list.c test_chashtable.c test_qtable.c test_utils.c
test_cds_LDADD = $(top_srcdir)/src/lib/libtsmapi.a

test_tsmapi_CFLAGS = -m64 -DLINUX_CLIENT -D_FILE_OFFSET_BITS=64 -D_LARGEFILE64_SOURCE -I$(top_srcdir)/src/lib -I@TSM_SRC_DIR@/ -I@LUSTRE_SRC_DIR@/lustre/include
bin_PROGRAMS += test_tsmapi
test_tsmapi_SOURCES = test_tsmapi.c CuTest.c test_utils.c
test_tsmapi_LDADD = $(top_srcdir)/src/lib/libtsmapi.a

ltsmbench_CFLAGS = -m64 -DLINUX_CLIENT -D_FILE_OFFSET_BITS=64 -D_LARGEFILE64_SOURCE -I$(top_srcdir)/src/lib -I@TSM_SRC_DIR@/
bin_PROGRAMS += ltsmbench
ltsmbench_SOURCES = ltsmbench.c test_utils.c
ltsmbench_LDADD = $(top_srcdir)/src/lib/libtsmapi.a
