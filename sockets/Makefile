SOURCE_DIR = src
SOURCE_P1 = $(SOURCE_DIR)/P1.c
SOURCE_P2 = $(SOURCE_DIR)/P2.c

OUT_DIR = build/output
TARGET_P1 = $(OUT_DIR)/P1
TARGET_P2 = $(OUT_DIR)/P2

all: 
	mkdir -p $(OUT_DIR)
	make $(TARGET_P1) $(TARGET_P2)

$(TARGET_P1):
		gcc $(SOURCE_P1) -o $(TARGET_P1)
$(TARGET_P2):
		gcc $(SOURCE_P2) -o $(TARGET_P2)


runP1:
		./$(TARGET_P1)
runP2:
		./$(TARGET_P2)


clean:
		rm -rf $(OUT_DIR)
