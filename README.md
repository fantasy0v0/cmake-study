```shell
cmake -B build -DCMAKE_BUILD_TYPE=Debug
cmake --build build
cmake --build build --target clean
cmake -B build -DCMAKE_BUILD_TYPE=Release
cmake --build build --config Release
cmake --build build --config Release --target clean
```