

DIRECTORY=Generated


build: .\vector-add-buffers.cpp
	icpx -fsycl -fintelfpga -DFPGA_EMULATOR .\vector-add-buffers.cpp -o $(DIRECTORY)\emu.exe

run: $(DIRECTORY)\emu.exe
	$(DIRECTORY)\emu.exe

clean:
	-if exist $(DIRECTORY) rmdir /S /Q $(DIRECTORY)
	mkdir $(DIRECTORY)