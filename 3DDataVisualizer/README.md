# 3D Voxel Data Visuzlier 

A python script to quickly view 3-dimensional scalar field data on IPython notebook. 

## How to use 

If you have a bit of experience in using python and matplotlib, the comment in the ipynb file would be enough and for you to figure out everything but it would be helpful to list up what the code expects from user. 

1. input data. Please take a look at sample input file (density.dat) and comments for the input data format.
```
datafile='density.dat'
```

2. give how many voxels in x,y, and z directions
```
nx=57; ny=57; nz=67
```

3. set the upper/lower limits of data to visualize and the range of color bar accordingly
```
vmin = 1; vmax = 4
```
```
# set the upper/lower limists in the plot. 
norm = colors.Normalize(vmin=vmin, vmax=vmax)
```

4. decide which dimension you want to slice the data
```
for idx in range(nx):
```

```
    im1 = ax1.imshow(xyz[idx][:][:], interpolation='none', origin='lower')
```
