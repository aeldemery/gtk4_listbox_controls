gtk4_listbox_controls_sources = [
  'main.vala',
  'window.vala',
]

gtk4_listbox_controls_deps = [
  dependency('gio-2.0', version: '>= 2.50'),
  dependency('gtk4', version: '>= 4.0.0'),
]

gnome = import('gnome')

gtk4_listbox_controls_sources += gnome.compile_resources('gtk4_listbox_controls-resources',
  'gtk4_listbox_controls.gresource.xml',
  c_name: 'gtk4_listbox_controls'
)

executable('gtk4_listbox_controls', gtk4_listbox_controls_sources,
  vala_args: '--target-glib=2.50',  dependencies: gtk4_listbox_controls_deps,
  install: true,
)
