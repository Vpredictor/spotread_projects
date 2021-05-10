# spotread_projects
## compile command
mex -R2018a -g spotread.c -L./ -linst -linstapp -lxicc -lgamut -lrspl -lcgats -licc -lplot -lvrml -lccast -laxtls -lyajl -lrender -ltiff -ljpeg -lpng -lz -lui -lnum -lucmm -ljcnf -lconv

## **usage: spotread(['options'],[logfile])**
|||
|:-:|:-:|
|'v'|Verbose mode| 
|'s'|Print spectrum for each reading|
|'S'|Plot spectrum for each reading|
|'c listno'|Set instrument port from the flowing list(default 1)|
|'t'|Use transmission measurement mode|
|'e'|Use emissive measurement mode|
|'eb'|Use display white brightness relative measurement mode|
|'ew'|Use display white point relative chromatically adjusted mode|
|'p'|Use telephoto measurement mode(absolute results)|
|'pb'|Use projector white brightness relative measurement mode|
|'pw'|Use projector white point relative chromatically adjusted mode|
|'a'|Use ambient measurement mode(absolute results)|
|'f'|Use ambient flash measurement mode (absolute results)|
|'w'|Use -i param. illuminant for comuting L*a*b*|
|'x'|Display Yxy instead Lab|
|'h'|Display Lch instead of Lab|
|'u'|Display Yuv instead of Lab|
|'V'|Show running average and std. devation from ref.|
|'T'|Display correlated color temperatures,CRI and TLCI|
|'N'|Disable auto calibration of instrument|
|'O'|Do one cal. or measure and exit|
|'H'|Start in high resolution spectrum mode (if available)|
|logfile|Optional file to save reading results as text|
