runoff_sources = [
  'main.c',
  'runoff-application.c',
  'runoff-window.c',
]

runoff_deps = [
  dependency('gtk4'),
  dependency('libadwaita-1', version: '>= 1.4'),
]

runoff_sources += gnome.compile_resources('runoff-resources',
  'runoff.gresource.xml',
  c_name: 'runoff'
)

executable('runoff', runoff_sources,
  dependencies: runoff_deps,
       install: true,
)
