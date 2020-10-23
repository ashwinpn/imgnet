# imgnet
Running NVIDIA profiler on the cloud 


## Usage
1. Change runtime type selecting GPU as hardware accelerator
2. Git clone this repository:
```
!git clone https://github.com/ashwinpn/imgnet.git
```
3. Change permissions:
```
!chmod 755 imgnet/INSTALL.sh
``` 
4. Install cuda, nvcc, gcc, and g++:
```
!./imgnet/INSTALL.sh
```
5. Add `/usr/local/cuda/bin` to `PATH`:
```python
import os
os.environ['PATH'] += ':/usr/local/cuda/bin'
```
6. Run 
```
!nvprof python main.py -a alexnet -b 8 --epochs 1 --lr 0.01 <Training and Validation folders parent directory>
```
