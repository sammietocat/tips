## This is a tips for update gcc/g++ to newer version(6.2) in ubuntu 16.04
The steps go as  
1. add the repository
```
  sudo apt-add-repository ppa:ubuntu-toolchain-r/test
```
![add repository](images/update-gcc/add-repo.png)  
2. install gcc 6
```
  sudo apt install gcc-6
```
![install gcc](images/update-gcc/install-gcc.png)  
3. install g++ 6
```
  sudo apt install g++-6
```
![install gcc](images/update-gcc/install-g++.png)  
4. update the corresponding alternative commands for default gcc and g++
```
  sudo update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-6 20
  sudo update-alternatives --install /usr/bin/g++ g++ /usr/bin/g++-6 20
```
![update alternative commands](images/update-gcc/update-cmd.png)  
5. update the configuration for gcc and g++ in case of multiple configure for gcc or g++
```
  sudo update-alternatives --config gcc
  sudo update-alternatives --config g++
```
![update configures](images/update-gcc/update-configure.png)  
-------
**Done**
