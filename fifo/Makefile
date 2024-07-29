SOURCE_DIR = src
SOURCE_P1 = $(SOURCE_DIR)/P1.c
SOURCE_P2 = $(SOURCE_DIR)/P2.c
SOURCE_FIFO = $(SOURCE_DIR)/fifoCreator.c

OUT_DIR = build/output

TARGET_P1 = P1
TARGET_P2 = P2
TARGET_FIFO = fifoCreator

all: 
	mkdir -p $(OUT_DIR)
	make $(TARGET_P1) $(TARGET_P2) $(TARGET_FIFO)

$(TARGET_P1):
		gcc $(SOURCE_P1) -o $(TARGET_P1)
$(TARGET_P2):
		gcc $(SOURCE_P2) -o $(TARGET_P2)
$(TARGET_FIFO):
		gcc $(SOURCE_FIFO) -o $(TARGET_FIFO)

runP1:
		./$(TARGET_P1)
runP2:
		./$(TARGET_P2)
init:
		./$(TARGET_FIFO)

clean:
		rm -f $(TARGET_P1) $(TARGET_P2) $(TARGET_FIFO)
		rm -rf $(OUT_DIR)
		rm -f /tmp/intFifo 
		rm -f /tmp/stringFifo