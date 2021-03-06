# LineCut analysis of polycrystalline graphene
Line cut method to estimate the average grain size of polycrystalline graphene.

### Author Information
Xiaoyi Liu, Email: xyliucd#foxmail.com. ORCID: https://orcid.org/0000-0002-3881-7740

*IMPORTANT: this program can be accurate when analyzing a polycrystalline graphene with over 25 grains. If the grains of polycrystalline graphene sheet are less than 25, you can count them handly.

[Ovito 3.0.0-dev422](https://www.ovito.org/) is used for the microstructure analysis of polycrystalline graphene, and we have added it into our environment modules. Thus, we can use it by the command below:
```
$ module load ovito/3.0.0dev
```
You should configure your ovito modulefiles accordingly. Or you can simply add the ovito directories into the environmental value PATH.

The usage of script "linecutGr.sh" is:
```
$ chmod +x linecutGr.sh
$ ./linecutGr.sh  [cfg file]   [Xsize]  [Ysize]  [interval]
```
Here "Xsize" and "Ysize" are the dimensions of a flat polycrystalline graphene.

A example is given below:
```
$ ./linecutGr.sh relax.90000.cfg 100 100 50
The average grain number along x-axis: 11.4706.
The average grain number along y-axis: 10.8824.

The average grain size along x-axis: 8.717939776.
The average grain size along y-axis: 9.189149452.

The average grain size: 8.950444208.
```
