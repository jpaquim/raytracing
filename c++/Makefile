open: build/image.ppm
	open build/image.ppm

build/image.ppm: build/main
	build/main > build/image.ppm

build/main: src/main.cpp src/color.hpp src/ray.hpp src/vec3.hpp
	mkdir -p build
	clang++ -std=c++2a src/main.cpp -o build/main

clean:
	rm -r build

.PHONY: run clean
