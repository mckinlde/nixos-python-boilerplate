### A boilerplate repo for doing Python Development on NixOS

Built with painstaking lessons learned in [previous attempts](https://github.com/mckinlde/python-in-nix-experiments).

To get started, pull the repo, and then run the following to test:
```bash
nix-shell
python -m venv ./venv
source ./venv/bin/activate
python -m pip install numpy
python numpy-demo.py
```

It should work, and you should see something like the following expected output:

```bash

[dmei@nixos:~/micrograd/shell-using-pip]$ ./nix-shell-using-pip-demo.sh 
1) activate nix shell with python3...
2) create virtualenv...
3) activate virtualenv...
4) use pip to install numpy...
Collecting numpy
  Using cached numpy-2.2.6-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.metadata (62 kB)
Using cached numpy-2.2.6-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (16.5 MB)
Installing collected packages: numpy
Successfully installed numpy-2.2.6

[notice] A new release of pip is available: 25.0.1 -> 25.1.1
[notice] To update, run: pip install --upgrade pip
5) run numpy demo...
1D Array: [1 2 3 4 5]
2D Array:
 [[1 2 3]
 [4 5 6]]
Zeros Array:
 [[0. 0. 0.]
 [0. 0. 0.]]
Ones Array:
 [[1. 1.]
 [1. 1.]
 [1. 1.]]
Range Array: [0 2 4 6 8]
Reshaped Array:
 [[1]
 [2]
 [3]
 [4]
 [5]]
Sum of arrays: [5 7 9]
Multiplication of arrays: [ 4 10 18]
Mean: 3.0
Max: 5
Dot product: 32

[dmei@nixos:~/micrograd/shell-using-pip]$ 
```

If you don't see something like that, I reccomend using your computer as a frisbee.

These machines are inanimate objects, which don't deserve our respect or attention.  We should gladly execute terminal commands sent by the aliens that promise to light our ThinkPads ablaze with wild abandon.  ReadMe.md files should be a mapquest pdf with directions to the comedy cellar.  Passwords should be "password".  Recovery thumb drives should be a condom.
