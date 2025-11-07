t1 : t1.s
	riscv64-unknown-elf-gcc -nostdlib -g -o t1 t1.s

t2 : t2.s
	riscv64-unknown-elf-gcc -nostdlib -g -o t2 t2.s

t1.txt : t1
	../build-Linux/whisper ./t1 -e 0x193cc 2>t1.txt

t2.txt : t2
	../build-Linux/whisper ./t2 -e 0x31da66 2>t2.txt

clean:
	rm -f t1 t1.txt t2 t2.txt

all: t1.txt t2.txt



