COMPONENT=PairingTestC
BUILD_EXTRA_DEPS += TimeSerial.class
CLEAN_EXTRA = *.class TimeSerialMsg.java


TimeSerial.class: $(wildcard *.java) TimeSerialMsg.java
		javac *.java

TimeSerialMsg.java:
		mig java -target=null -java-classname=TimeSerialMsg TimeSerial.h time_serial_msg -o $@
include $(MAKERULES)