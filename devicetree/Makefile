
dtbs: 
	mkdir -p ./out &> /dev/null
	rm -R ./out/* &> /dev/null &
	wait

	cpp -nostdinc -I include -I ./  -undef -x assembler-with-cpp  sun8i-h3-redboxmini.dts ./out/preprocessed
	dtc -I dts -O dtb -p 0x1000 ./out/preprocessed -o ./out/dtb

	mv ./out/dtb ./out/sun8i-h3-redboxmini.dtb
	cp ./out/sun8i-h3-redboxmini.dtb ../
