project(
    'insight',
    'c',
    version: '1.0.0',
    license: 'MIT'
)

buildtype = 'release'

install_headers('include/insight.h')

insight_lib = shared_library(
    'insight',
    'source/insight.c',
    install: true
)

insight_dep = declare_dependency(link_with: insight_lib)

pkg = import('pkgconfig')
pkg.generate(insight_lib)
