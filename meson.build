project('tetgen', 'cpp', version : '1.6.0')

tetgen_inc = include_directories('.')

tetgen_lib = static_library(
  'tetgen',
  ['tetgen.cxx', 'predicates.cxx'],
  cpp_args : ['-DTETLIBRARY']
)

tetgen_dep = declare_dependency(
  link_with : tetgen_lib,
  include_directories : tetgen_inc
)

meson.override_dependency('tetgen', tetgen_dep)
meson.override_dependency('tetgen-1.6.0', tetgen_dep)
