# testing-cpp-package-manager
testing some example c/c++ package managers

# Install Conan
Follow the [conan installation page](https://docs.conan.io/en/latest/installation.html) to install conan.

# With Conan
```
pushd conan
mkdir build
cd build && conan install .. [--build=missing]
cmake ..
make
./bin/formater 
popd
```