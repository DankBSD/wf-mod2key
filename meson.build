project('wf-mod2key', ['cpp'], version: '0.0.1', license: 'Unlicense',
	default_options: ['cpp_std=c++17', 'warning_level=2'])

wayfire = dependency('wayfire')
wlroots = dependency('wlroots', fallback: ['wlroots', 'wlroots'])

plugin_gsettings = shared_module('mod2key', 'mod2key.cpp',
	dependencies: [wayfire, wlroots],
	install: true,
	install_dir: 'lib/wayfire')

install_data('mod2key.xml', install_dir: 'share/wayfire/metadata')
