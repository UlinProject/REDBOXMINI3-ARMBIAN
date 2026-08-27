# make
# OR:
# make default-noturbo
# make turbomod

OUT_DIR   := ./out
CPP_FLAGS := -nostdinc -I include -I ./ -undef -x assembler-with-cpp
DTC_FLAGS := -I dts -O dtb -p 0x1000

.PHONY: default all default-noturbo turbomod clean

default: default-noturbo

all: default-noturbo turbomod

default-noturbo: build-noturbodef
turbomod: build-turbo

build-%: sun8i-h3-redboxmini-%.dts
	@echo "============================================="
	@echo " [BUILD] Configuration: $*"
	@echo " [FROM]  $<"
	@echo "============================================="
	@echo ""
	@mkdir -p $(OUT_DIR)
	@rm -rf $(OUT_DIR)/*

	cpp $(CPP_FLAGS) $< $(OUT_DIR)/preprocessed
	dtc $(DTC_FLAGS) $(OUT_DIR)/preprocessed -o $(OUT_DIR)/sun8i-h3-redboxmini.dtb

	@echo " [COPY]  Output file copied to: ../sun8i-h3-redboxmini.dtb"
	@cp $(OUT_DIR)/sun8i-h3-redboxmini.dtb ../
	@echo " [DONE]  Build for $* completed successfully."
	@echo ""

clean:
	rm -rf $(OUT_DIR)
