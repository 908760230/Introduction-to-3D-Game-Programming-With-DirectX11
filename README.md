Introduction-to-3D-Game-Programming-With-DirectX11
==================================================

Book Example Code in [Introduction to 3D Game Programming With DirectX11 by Frank Luna ]
http://www.d3dcoder.net/



New Project setup:
==================

Do not modify the relative directory structure of these samples.  In particular, for each 
project sample, the Common folder must be obtained from it via "../../Common".

Debug libraries:
----------------

d3d11.lib;d3dx11d.lib;D3DCompiler.lib;Effects11d.lib;dxerr.lib;dxgi.lib;dxguid.lib;%(AdditionalDependencies)

Release libraries:
------------------

d3d11.lib;d3dx11.lib;D3DCompiler.lib;Effects11.lib;dxerr.lib;dxgi.lib;dxguid.lib;%(AdditionalDependencies)

C/C++ Additional Include Directories:
-------------------------------------

1) Path to DirectX Header files.

2) ../../Common (or Absolute Path to Common)

Linker Additional Library Directories:
--------------------------------------

1) Path to DirectX Library files.

2) ../../Common (or Absolute Path to Common)

FXC Call
--------

a) Debug mode:   fxc /Fc /Od /Zi /T fx_5_0 /Fo "%(RelativeDir)\%(Filename).fxo" "%(FullPath)"
b) Release mode: fxc /T fx_5_0 /Fo "%(RelativeDir)\%(Filename).fxo" "%(FullPath)"

a) Debug Description: fxc compile for debug: %(FullPath)
b) Release Description: fxc compile for release: %(FullPath)

Outputs: %(RelativeDir)\%(Filename).fxo


Compile Error
---------------
- Effects11d.lib ��ũ ����
C:\Program Files\Microsoft DirectX SDK (June 2010)\Samples\C++\Effects11 
������Ʈ�� �������ؼ� ��ũ����.


- DirectX 11 �ʱ�ȭ ����
�Ʒ� ����Ʈ�� ��������.
http://stackoverflow.com/questions/10586956/what-can-cause-d3d11createdevice-to-fail-with-e-fail

