ICONS=package rainbow_apple power

TARGET_DIR=~/.dt/icons

all: $(foreach f,$(ICONS), $(TARGET_DIR)/$(f).l.pm $(TARGET_DIR)/$(f).m.pm)
#all: $(foreach f,$(ICONS),$(f).48.xpm $(f).32.xpm)

%.48.xpm: %.png
	convert -resize 48x48 -format xpm $< $@
%.32.xpm: %.png
	convert -resize 32x32 -format xpm $< $@


$(TARGET_DIR)/%.l.pm: %.48.xpm
	cp $< $@
$(TARGET_DIR)/%.m.pm: %.32.xpm
	cp $< $@
