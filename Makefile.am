AUTOMAKE_OPTIONS = foreign

dist_bin_SCRIPTS = my_program
CLEANFILES = $(dist_bin_SCRIPTS)

my_program: Makefile
	echo "#!/usr/bin/env ruby" > $@
	echo "puts 'Hello world'" >> $@
	chmod +x $@
