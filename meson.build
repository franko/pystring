project('pystring', 'cpp', default_options : ['cpp_std=c++11'])

libpystring = library('pystring', 'pystring.cpp', install: true)
install_headers('pystring.h')

pkg = import('pkgconfig')
pkg.generate(libpystring,
    filebase : 'libpystring',
    name : 'libpystring',
    libraries : libpystring,
    description : 'C++ string library with a python-like interface',
    url : 'github.com/imageworks/pystring',
)
