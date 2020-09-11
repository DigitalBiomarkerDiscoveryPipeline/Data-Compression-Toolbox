# Method #4: DCT based DOST + Huffman encoding

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

If you use this method in your work, please cite the DBDP: dbdp.org and the references at the bottom of this page.

This method uses Butterworth filter and resampling to preprocess the raw data. And then DCT based DOST was applies on the data. After this step and some basic quantization, Huffman encoding will be applied on the processed data.

The detailed steps and instructions are listed in the code by comments and markdown trunks.


### Instructions

Input the signal to be compressed and define the parameters listed below

1. Sampling frequency
2. Decimal in quantization
3. Useful length of the signal
4. Name of the saved files


Dependencies:

```sh
matplotlib.pyplot
pandas
numpy
scipy
os
```

### Evaluation

The results of this method on the following wearable sensors:

| Wearable Sensor | Compression Ratio | Percentage RMS difference |
| ------ | ------ | ------ | 
| ECG | 57.46 | 8.97 |
| PPG | 35.74 | 0.44 |
| ACC | 41.86 | 3.66 |
| EDA | 25.22 | 0.08 |
| TEMP | 12.61 | 5.28 |



### References

Jha, Chandan & Kolekar, Maheshkumar. (2018). Electrocardiogram data compression using DCT based discrete orthogonal Stockwell transform. Biomedical Signal Processing and Control. 46. 174-181. 10.1016/j.bspc.2018.06.009.

tcmpr 0.2, Konrad Poreba: https://tcmpr.readthedocs.io/en/latest/index.html
PyPI: https://pypi.org/project/tcmpr/


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
