project(
    'LedController-examples-raspi',
    'c', 
    'cpp',
    default_options : [
        'c_std=c11', 
        'cpp_std=c++17',
        'b_lto=true',
        'b_pgo=generate',
        'b_coverage=false',
    ],
    version:'1.0.0',
    meson_version: '>= 0.54.0',
)

deps = [
    dependency('LedController', required: true, fallback: 'LedController'),
]

incdir = include_directories('.')

sources = [
    'main.cpp',
#    'Led-matrix-rocket.cpp',
    '7-Segment-couting.cpp',
]

executable(
    'example',
    sources,
    include_directories : incdir,
    dependencies: deps,
    install : true,
)
