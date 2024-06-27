project('v meson setup', version : '0.0.1')

comp = find_program('v')

# infile = 'src/main.v'
outfile = 'app'

mytarget = custom_target('targetname',
  output : outfile,
  # input : infile,
  command : [comp, join_paths(meson.current_source_dir(), get_option('src_code_path')), '-o', '@OUTPUT@'],
  install : true,
  install_dir : join_paths(meson.current_source_dir(), get_option('install_path')))

