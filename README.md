# spotread_projects
## compile command
mex -R2018a -g spotread.c -L./ -linst -linstapp -lxicc -lgamut -lrspl -lcgats -licc -lplot -lvrml -lccast -laxtls -lyajl -lrender -ltiff -ljpeg -lpng -lz -lui -lnum -lucmm -ljcnf -lconv

## **usage: spotread(['options'],[logfile])**
|'options'|'meaning'|
|:-:|:-:|
|'printDebug',[level]|Print debug diagnostics to stderr ,level is an integer range from 0 to 9,default is 1|
|'?'|Show detail information about usage|
|'verboseMode'|Verbose mode| 
|'showSpectrum',[type]|Print spectrum for each reading,type is an integer range from 1 to 2,default is 1,1:print spectrum for each reading,2:plot spectrum for each reading|
|'comPort',portnum|Set instrument port from the following list(default 1), portnum is an integer range from 1 to 40|
|'displayType',type|Display type, type is a positive integer (to do)|
|'setSimulatedInst',inst|Simulated instrument illumination (FWA),inst is a filename or an integer range from 0 to 7,0:"A" or "M0",1:"C",2:"D50" or "M1",3:"D50M2" or "M2",4:"D65",5:"F5",6:"F8",7:"F10"|
|'spectralIlluminantType',inst|Spectral Illuminant type for XYZ computation,inst is filename or an integer range from 0 to 7,0:"A",1:"C",2:"D50",3:"D50M2",4:"D65",5:"F5",6:"F8",7:"F10"|
|'useIParam'|Use -i illuminant for L*a*b conversion|
|'chooseCIEObserver',type|Spectral Observer type,type is a filename or an integer range from 0 to 6,0:"1931_2",1:"1964_10",2:"2012_2",3:"2012_10",4:"1955_2",5:"1978_2",6:"shaw"|
|'measureMode',mode|mode is an integer range from 0 to 8,0:use emissive measurement mode(absolute results),1:use display white brightness relative measurement mode,2:use display white point relative chromatically adjusted mode,3:use transmission measurement mode,4:use telephoto measurement mode(absolute results),5:use projector white brightness relative measurement mode,6:use projector white point relative chromatically adjusted mode,7:use ambient measurement mode(absolute results),8:use ambient flash measurement mode(absolute results)|
|'filterConfig',config|Set filter configuration,config is an integer range from 0 to 3,0:None,1:Polarising filter,2:D65,3:U.V. Cut|
|'E',file|Extra filter compensation file,file is a file name|
|'xrgaConversion',param|XRGA conversion,param is an integer range from 0 to 3,0:N,1:A,2:X,3:G|
|'Display',param|param is an integer range from 0 to 2,0:Display Yxy instead Lab,1:Display Lch instead of Lab,2:Display Yuv instead of Lab|
|'computeAvgAndDev'|Compute running average and standard deviation from ref.Also turns off clamping|
|'showCCT'|Show CCT etc|
|'showDensities'|Show densities|
|'nAutoCal'|Disable auto calibration of instrument|
|'calOrMeasure',param|Do one cal. or measure and exit,param is a file name|
|'highResMode'|High res mode|
|'X',param|Colorimeter Correction Matrix or Colorimeter Calibration Spectral Samples,param is a file name|
|'presetReferenceSpect',param|Present reference spectrum,param is a file name|
|'extraFlags',param|Extra flags|
|'serialPort',param|Override serial port flow control,param is an integer range from 0 to 2,0:none,1:HW,2:Xon/Xoff|
|logfile|Optional file to save reading results as text|
