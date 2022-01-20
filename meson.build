lmdb = declare_dependency(
  link_with: static_library(
    'lmdb',
    [
      'lmdb/libraries/liblmdb/mdb.c',
      'lmdb/libraries/liblmdb/midl.c',
    ],
    c_args: [
      '-DNTSTATUS=LONG',
    ],
    override_options: [
      'warning_level=0',
      'werror=false',
      'c_std=c11',
    ],
    include_directories: include_directories('lmdb/libraries/liblmdb'),
  ),
  include_directories: include_directories('lmdb/libraries/liblmdb'),
)
