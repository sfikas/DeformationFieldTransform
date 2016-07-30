# *UNDER CONSTRUCTION*

## DeformationFieldTransform

A C++ app that uses a 3D deformation field (field of 3D vectors) to warp/deform an input 3D volume.

## Requirements

This app has been requires [ITK]. 
It has been tested with [ITK] version 4.11.

## Build

Run the following to build:

```
cd DeformationFieldTransform/
cmake .
make
```

## Run

You need a 3D volume as input, plus a deformation field which will be used to warp/deform the input volume.
An output volume will be produced containing the result.
Run with:
```
DeformationFieldTransform <Input volume> <Input deformation field> <Output volume>
```

Example:
```
DeformationFieldTransform MRIscan_0001.nii deformationfield.mha MRIscan_0001.output.nii
```

## Miscellaneous

### Difference between ITK's WarpImageFilter and DeformationFieldTransform/DisplacementFieldTransform

* http://public.kitware.com/pipermail/insight-users/2011-July/041853.html
* https://itk.org/pipermail/insight-users/2011-May/041192.html
* https://itk.org/Doxygen/html/classitk_1_1DisplacementFieldTransform.html
* https://itk.org/Doxygen/html/classitk_1_1InverseDisplacementFieldImageFilter.html
* https://itk.org/Doxygen/html/classitk_1_1WarpImageFilter.html

[ITK]: <https://itk.org/>
