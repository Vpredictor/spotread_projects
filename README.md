# spotread_projects
## compile command
mex -R2018a -g spotread.c -L./ -linst -linstapp -lxicc -lgamut -lrspl -lcgats -licc -lplot -lvrml -lccast -laxtls -lyajl -lrender -ltiff -ljpeg -lpng -lz -lui -lnum -lucmm -ljcnf -lconv

## **usage: spotread(['options'],[logfile])**
|'options'|'meaning'|
|:-:|:-:|
|'printDebug',[level]|Print debug diagnostics to stderr ,level is an integer range from 0 to 9,default is 1|
|'?'|Show detail information about usage|
|'verboseMode'|Verbose mode| 
|'showSpectrum',[type]|Print spectrum for each reading,type is an integer range from 1 to 2,default is 1|
|'comPort',portnum|Set instrument port from the following list(default 1), portnum is an integer range from 1 to 40|
|'displayType',type|Display type, type is an integer (to do)|
|'setSimulatedInst',inst|Simulated instrument illumination (FWA),inst is instrument name or filename|
|'spectralIlluminantType',inst|Spectral Illuminant type for XYZ computation,inst is instrument name or filename|
|'useIParam'|Use -i illuminant for L*a*b conversion|
|'chooseCIEObserver',type|Spectral Observer type|
|'measureMode',mode|mode is an integer range from 0 to 10|
|'filterConfig',config|config is an integer range from 0 to 3|
|'E','file'|Extra filter compensation file,file is a file name|
|'xrgaConversion',param|XRGA conversion,param is an integer range from 0 to 3|
|'Display',param|param is an integer range from 0 to 2,0:Display Yxy instead Lab,1:Display Lch instead of Lab,2:Display Yuv instead of Lab|
|'computeAvgAndDev'|Compute running average and standard deviation from ref.Also turns off clamping|
|'showCCT'|Show CCT etc|
|'showDensities'|Show densities|
|'manualCal',param|manual calibration,param range from 0 to 9|
|'nAutoCal'|No auto calibration|
|'calOrMeasure','param'|Do one cal. or measure and exit,param is a file name|
|'highResMode'|High res mode|
|'X','param'|Colorimeter Correction Matrix or Colorimeter Calibration Spectral Samples,param is a file name|
|'presetReferenceSpect','param'|Present reference spectrum,param is a file name|
|'extraFlags','param'|Extra flags|
|'serialPort',param|Serial port flow control,param is an integer range from 0 to 2|
|logfile|Optional file to save reading results as text|
