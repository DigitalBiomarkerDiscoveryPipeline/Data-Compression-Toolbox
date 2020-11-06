# Discrete Wavelet Transform + Run Length Encoding

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

If you use this method in your work, please cite the DBDP: dbdp.org and the references at the bottom of this page.

This method utilizes a discrete wavelet transform to decompose a signal into its approximation and detail wavelet coefficients. After thresholding, these coefficients are further compressed through simple bit packing and run length encoding.


### Instructions

Input the signal to be compressed and define the various paramters listed below:  
1. sampling rate
1. maximum number of bits that can represent run length
1. maximum desired PRD
1. threshold percentage for approximation coefficients
1. threshold percentage for detail 5 coefficients
1. threshold percentage for detail 4-1 coefficients


*note: the do_plot parameter is for visualization purposes only. as such, the plotting functionality is omitted in the comprehensive frame function.*

```sh
Code can go here if you need that for your instructions
```

Dependencies:

```sh
matplotlib.pyplot
pywt
numpy
pandas
scipy.signal
copy
json
os
```

### Evaluation

The results of this method on the following wearable sensors:

| Wearable Sensor | Compression Ratio | Percentage RMS difference |
| ------ | ------ | ------ | 
| ECG | 137.39 | 0.85% |
| PPG | 16.66 | 1.34% |
| ACC | 14.94 | 0.94% |
| EDA | 15.43 | 0.53% |
| TEMP | 78.77 | 0.10% |



### References

Python code from the following Github was used and modified:
https://github.com/nerajbobra/wavelet-based-ecg-compression  
Methodology was derived from the following paper:
[An efficient coding algorithm for the compression of ECG signals using the wavelet transform](https://ieeexplore.ieee.org/document/991163)  
With some modifications made according to this paper:
[Comments on "An efficient coding algorithm for the compression of ECG signals using the wavelet transform"](https://ieeexplore.ieee.org/document/1213856)

License
----

MIT



[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)


   [dill]: <https://github.com/joemccann/dillinger>
   [git-repo-url]: <https://github.com/joemccann/dillinger.git>
   [john gruber]: <http://daringfireball.net>
   [df1]: <http://daringfireball.net/projects/markdown/>
   [markdown-it]: <https://github.com/markdown-it/markdown-it>
   [Ace Editor]: <http://ace.ajax.org>
   [node.js]: <http://nodejs.org>
   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
   [jQuery]: <http://jquery.com>
   [@tjholowaychuk]: <http://twitter.com/tjholowaychuk>
   [express]: <http://expressjs.com>
   [AngularJS]: <http://angularjs.org>
   [Gulp]: <http://gulpjs.com>

   [PlDb]: <https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md>
   [PlGh]: <https://github.com/joemccann/dillinger/tree/master/plugins/github/README.md>
   [PlGd]: <https://github.com/joemccann/dillinger/tree/master/plugins/googledrive/README.md>
   [PlOd]: <https://github.com/joemccann/dillinger/tree/master/plugins/onedrive/README.md>
   [PlMe]: <https://github.com/joemccann/dillinger/tree/master/plugins/medium/README.md>
   [PlGa]: <https://github.com/RahulHP/dillinger/blob/master/plugins/googleanalytics/README.md>
