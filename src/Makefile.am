DEBUG_FLAGS = -D_GNU_SOURCE

if DEBUG
DEBUG_FLAGS += -g -O0
endif

lib_LTLIBRARIES=libmgStd.la 
libmgStd_la_CFLAGS=$(DEBUG_FLAGS) -fPIC -shared -D_LARGEFILE64_SOURCE=1 -std=c99 
libmgStd_la_LIBADD=
libmgStd_la_SOURCES=mglist.c mgmurmurhash.c mgtime.c mgmd5.c mgsha1.c mgbase64.c mgsha256.c mgsha384.c mgsha512.c mgcrc32.c mgbstree.c mgsplaytree.c mgavltree.c mgrbtree.c mgprocess_rate.c mghmac_md5.c mgfastsort.c mgstack.c
libmgStd_HEADERS=mglist.h mgmurmurhash.h mgtime.h mgmd5.h mgsha1.h mgbase64.h mgsha256.h mgsha384.h mgsha512.h mgcrc32.h mgbstree.h mgsplaytree.h mgavltree.h mgrbtree.h mgprocess_rate.h mghmac_md5.h mgfastsort.h mgstack.h
libmgStddir=@includedir@/mgStd

#bin_PROGRAMS=mglist_test
noinst_PROGRAMS=mglist_test mgmurmurhash_test mgmd5_test mghlist_test mgsha1_test mgbase64_test mgsha256_test mgsha384_test mgsha512_test mgcrc32_test mgbstree_test mgsplaytree_test mgavltree_test mgrbtree_test mghmac_md5_test mgstack_test

mglist_test_DEPENDENCIES=./libmgStd.la
mglist_test_CFLAGS = -I./
mglist_test_LDADD=./libmgStd.la
mglist_test_SOURCES=test/mglist_test.c
mglist_test_LDFLAGS= $(DEBUG_FLAGS)

mghlist_test_DEPENDENCIES=./libmgStd.la
mghlist_test_CFLAGS = -I./
mghlist_test_LDADD=./libmgStd.la
mghlist_test_SOURCES=test/mghlist_test.c
mghlist_test_LDFLAGS=$(DEBUG_FLAGS)

mgmurmurhash_test_DEPENDENCIES=./libmgStd.la
mgmurmurhash_test_LDADD=./libmgStd.la
mgmurmurhash_test_CFLAGS = -I./
mgmurmurhash_test_SOURCES=test/mgmurmurhash_test.c
mgmurmurhash_test_LDFLAGS=$(DEBUG_FLAGS)

mgmd5_test_DEPENDENCIES=./libmgStd.la
mgmd5_test_LDADD=./libmgStd.la
mgmd5_test_CFLAGS = -I./
mgmd5_test_SOURCES=test/mgmd5_test.c
mgmd5_test_LDFLAGS=$(DEBUG_FLAGS)

mgsha1_test_DEPENDENCIES=./libmgStd.la
mgsha1_test_LDADD=./libmgStd.la
mgsha1_test_CFLAGS = -I./
mgsha1_test_SOURCES=test/mgsha1_test.c
mgsha1_test_LDFLAGS=$(DEBUG_FLAGS)

mgsha256_test_DEPENDENCIES=./libmgStd.la
mgsha256_test_LDADD=./libmgStd.la
mgsha256_test_CFLAGS = -I./
mgsha256_test_SOURCES=test/mgsha256_test.c
mgsha256_test_LDFLAGS=$(DEBUG_FLAGS)

mgsha384_test_DEPENDENCIES=./libmgStd.la
mgsha384_test_LDADD=./libmgStd.la
mgsha384_test_CFLAGS = -I./
mgsha384_test_SOURCES=test/mgsha384_test.c
mgsha384_test_LDFLAGS=$(DEBUG_FLAGS)

mgsha512_test_DEPENDENCIES=./libmgStd.la
mgsha512_test_LDADD=./libmgStd.la
mgsha512_test_CFLAGS = -I./
mgsha512_test_SOURCES=test/mgsha512_test.c
mgsha512_test_LDFLAGS=$(DEBUG_FLAGS)

mgbase64_test_DEPENDENCIES=./libmgStd.la
mgbase64_test_LDADD=./libmgStd.la
mgbase64_CFLAGS = -I./
mgbase64_test_SOURCES=test/mgbase64_test.c
mgbase64_test_LDFLAGS=$(DEBUG_FLAGS)

mgcrc32_test_DEPENDENCIES=./libmgStd.la
mgcrc32_test_LDADD=./libmgStd.la
mgcrc32_test_CFLAGS = -I./
mgcrc32_test_SOURCES=test/mgcrc32_test.c
mgcrc32_test_LDFLAGS=$(DEBUG_FLAGS)

mgbstree_test_DEPENDENCIES=./libmgStd.la
mgbstree_test_LDADD=./libmgStd.la
mgbstree_test_CFLAGS = -I./
mgbstree_test_SOURCES=test/mgbstree_test.c
mgbstree_test_LDFLAGS=$(DEBUG_FLAGS)

mgavltree_test_DEPENDENCIES=./libmgStd.la
mgavltree_test_LDADD=./libmgStd.la
mgavltree_test_CFLAGS = -I./
mgavltree_test_SOURCES=test/mgavltree_test.c
mgavltree_test_LDFLAGS=$(DEBUG_FLAGS)

mgsplaytree_test_DEPENDENCIES=./libmgStd.la
mgsplaytree_test_LDADD=./libmgStd.la
mgsplaytree_test_CFLAGS = -I./
mgsplaytree_test_SOURCES=test/mgsplaytree_test.c
mgsplaytree_test_LDFLAGS=$(DEBUG_FLAGS)

mgrbtree_test_DEPENDENCIES=./libmgStd.la
mgrbtree_test_LDADD=./libmgStd.la
mgrbtree_test_CFLAGS = -I./
mgrbtree_test_SOURCES=test/mgrbtree_test.c
mgrbtree_test_LDFLAGS=$(DEBUG_FLAGS)

mghmac_md5_test_DEPENDENCIES=./libmgStd.la
mghmac_md5_test_LDADD=./libmgStd.la
mghmac_md5_CFLAGS = -I./
mghmac_md5_test_SOURCES=test/mghmac_md5_test.c
mghmac_md5_test_LDFLAGS=$(DEBUG_FLAGS)

mgstack_test_DEPENDENCIES=./libmgStd.la
mgstack_test_LDADD = ./libmgStd.la
mgstack_test_CFLAGS = -I./
mgstack_test_SOURCES = test/mgstack_test.c
mgstack_test_LDFLAGS = $(DEBUG_FLAGS)
