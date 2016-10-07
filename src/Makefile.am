AUTOMAKE_OPTIONS=foreign
bin_PROGRAMS=twinkle
twinkle_SOURCES=\
				pmd/pmdMain.cpp \
				bson/src/bsonobj.cpp bson/src/util/json.cpp bson/src/oid.cpp \
				bson/src/lib/base64.cpp bson/src/lib/md5.cpp bson/src/lib/nonce.cpp

twinkle_CXXFLAGS=-I../boost -Ibson/src -Iinclude -D_FILE_OFFSET_BITS=64 -ggdb -Wall -O0
twinkle_LDADD=-lpthread -lm -lboost_system -lboost_thread -lboost_program_options
twinkle_LDFLAGS=-fPIC -rdynamic -L../boost/stage/lib -pthread
