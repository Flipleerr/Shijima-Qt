include ../../common.mk

SOURCES = Platform.mm ActiveWindowObserver.cc PrivateActiveWindowObserver.mm
QT_LIBS = Core Widgets
CXXFLAGS += -x objective-c++ -fobjc-arc -arch x86_64

all:: macOS.a

macOS.a: $(OBJECTS)
	rm -f $@
	$(AR) rcs $@ $(OBJECTS)

clean::
	rm -f $(OBJECTS) macOS.a
