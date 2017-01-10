bitday_pics = 01-Early-Morning.png \
	      02-Mid-Morning.png \
	      03-Late-Morning.png \
	      04-Early-Afternoon.png \
	      05-Mid-Afternoon.png \
	      06-Late-Afternoon.png \
	      07-Early-Evening.png \
	      08-Mid-Evening.png \
	      09-Late-Evening.png \
	      10-Early-Night.png \
	      11-Mid-Night.png \
	      12-Late-Night.png

backgrounddir = $(datadir)/backgrounds/bitday
background_DATA = $(bitday_pics) bitday-timed.xml

metadatadir = $(datadir)/gnome-background-properties
metadata_DATA = bitday.xml

CLEANFILES = bitday.xml bitday-timed.xml

EXTRA_DIST = $(bitday_pics) bitday.xml.in bitday-timed.xml.in

bitday.xml: bitday.xml.in Makefile
	$(AM_V_GEN) sed -e 's^\@datadir\@^$(datadir)^g' < $(srcdir)/bitday.xml.in > bitday.xml.tmp \
	&& mv bitday.xml.tmp bitday.xml

bitday-timed.xml: bitday-timed.xml.in Makefile
	$(AM_V_GEN) sed -e 's^\@datadir\@^$(datadir)^g' < $(srcdir)/bitday-timed.xml.in > bitday-timed.xml.tmp \
	&& mv bitday-timed.xml.tmp bitday-timed.xml

MAINTAINERCLEANFILES = Makefile.in
