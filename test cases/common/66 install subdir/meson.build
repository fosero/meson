project('install a whole subdir', 'c')

# A subdir with an exclusion:
install_subdir('sub2',
  exclude_files : ['excluded-three.dat'],
  exclude_directories : ['excluded'],
  install_dir : 'share')

subdir('subdir')
# A subdir with write perms only for the owner
# and read-list perms for owner and group
install_subdir('sub1', install_dir : 'share', install_mode : ['rwxr-x--t', 'root'])
install_subdir('sub/sub1', install_dir : 'share')
