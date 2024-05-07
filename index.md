# Robust Low-Poly Meshing for General 3D Models
**Zhen Chen<sup>1,2</sup>, Zherong Pan<sup>1</sup>, Kui Wu<sup>1</sup>, Etienne Vouga<sup>2</sup>, Xifeng Gao<sup>1</sup>**

<sup>1</sup>Lightspeed Studios, <sup>2</sup>Univeristy of Texas at Austin

*ACM Transactions on Graphics (SIGGRAPH), 2023*
![](imgs/gallery_24dpi.jpg)

[Paper](paper/Robust_Self_Collision_Free_Remeshing.pdf) [Program](exe/RoLoPM_EXE.zip) [data](https://www.dropbox.com/scl/fo/9smmsvajzn4qj23s9xfoj/h?rlkey=g27cj058urro6rroqb1zffmxz&dl=0)

## Abstract
<p style="text-align: justify;">
We propose a robust re-meshing approach that can automatically generate visual-preserving low-poly meshes for any high-poly models found in the wild. Our method can be seamlessly integrated into current mesh-based 3D asset production pipelines. Given an input high-poly, our method proceeds in two stages: 1) Robustly extracting an offset surface mesh that is feature-preserving, and guaranteed to be watertight, manifold, and self-intersection free; 2) Progressively simplifying and flowing the offset mesh to bring it close to the input. The simplicity and the visual-preservation of the generated low-poly is controlled by a user-required target screen size of the input: decreasing the screen size reduces the element count of the low-poly but enlarges its visual difference from the input. We have evaluated our method on a subset of the Thingi10K dataset that contains models created by practitioners in different domains, with varying topological and geometriccomplexities. Compared to state-of-the-art approaches and widely used software, our method demonstrates its superiority in terms of the element count, visual preservation, geometry, and topology guarantees of the generated low-polys.
</p>

## News
Our surface remeshing exe is released! Check [here](exe/RoLoPM_EXE.zip) for details. 

## Run Exe
To execute our executable file, follow these steps:

```
./SurfaceRemeshingCli_bin.exe -i "YourObjMeshFile.obj" -n 100
```

Here's what each option means:

- The `-i` flag specifies the input mesh file in .obj format.
- The `-n` flag allows you to adjust precision. A higher number yields a more precise result but consumes more time and memory. Please note that the current version supports a maximum precision level of `-n 400`.

For more detailed information about available parameters, you can run:

```
./SurfaceRemeshingCli_bin.exe -h
```

This command will provide you with comprehensive details on the available options and their usage. 


## License

# Software License Agreement

**IMPORTANT: PLEASE READ THE TERMS AND CONDITIONS OF THIS LICENSE AGREEMENT CAREFULLY BEFORE CONTINUING WITH THIS PROGRAM INSTALL: [Tencent Holdings Ltd]'s ("Licensor") "Software" includes all software included with this agreement, the associated media, any printed materials, and any "online" or electronic documentation. By installing, copying, or otherwise using the Software, you agree to be bound by the terms of this agreement. If you do not agree to the terms of this agreement, promptly uninstall this software.**

## LICENSE TERMS

The Licensor grants you a non-exclusive, non-transferable license to use the Software subject to all the terms and conditions set forth here.

1. **Use of the Software**
    - You may install and use an unlimited number of copies of the Software on your devices.
    - The primary user of the device on which the Software is installed may make a second copy for their exclusive use on a portable device.
    - You are allowed to use the Software for any lawful purpose.

2. **Restrictions**
    - You may not modify, translate, rent, sublicense, lease, lend, resell for profit, distribute, network, or create derivative works based upon the Software or any part thereof.
    - You shall not merge, adapt, translate, modify, or reverse engineer, decompile, disassemble or create derivative works of the Software and shall not permit others to do so.
    - You may not redistribute the Software in any way, including by means of uploading the Software to a file sharing service or other type of hosting service or distributing the Software through any other medium.

3. **Termination**
    - This License is effective until terminated. You may terminate it at any time by destroying the Software, together with all copies thereof.
    - This License will also terminate automatically if you fail to comply with any term or condition of this Agreement. Upon such termination, you agree to destroy the Software, together with all copies thereof.
  
4. **Copyright**
    - The Software is owned by the Licensor and is protected by United States copyright law and international treaty provisions.

5. **No Warranties**
    - The Licensor expressly disclaims any warranty for the Software. The Software and any related documentation is provided "as is" without warranty of any kind, either express or implied, including, without limitation, the implied warranties or merchantability, fitness for a particular purpose, or noninfringement.
    - The entire risk arising out of use or performance of the Software remains with you.

6. **Limitation of Liability**
    - In no event shall the Licensor be liable for any damages (including, without limitation, lost profits, business interruption, or lost information) rising out of 'Authorized Users' use of or inability to use the Software, even if the Licensor has been advised of the possibility of such damages. In no event will Licensor be liable for loss of data or for indirect, special, incidental, consequential (including lost profit), or other damages based in contract, tort or otherwise.

7. **Governing Law**
    - This agreement shall be governed by the laws of the State/Province of [Your State/Province], without reference to conflict of laws principles.

**By installing and using the Software, you acknowledge that you have read this agreement, understand it, and agree to be bound by its terms and conditions.**
