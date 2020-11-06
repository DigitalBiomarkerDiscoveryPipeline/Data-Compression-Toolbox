# Singular Value Decomposition + Huffman

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

If you use this method in your work, please cite the DBDP: dbdp.org and the references at the bottom of this page.

This method uses Butterworth filter and resampling to preprocess the raw data. And then applies the singular value decomposition on the data and tuning the rank of sigma to reach a good performance. After this step, the quantized data will be Huffman encoded.


### Instructions

Put instructions of how to use your method here.

1. Sampling frequency
2. Rank of Sigma after SVD
3. Decimal in quantization
4. Useful length of the signal
5. Name of the saved files
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
| ECG | 50.22 | 0.38% |
| PPG | 5.41 | 0.48% |
| ACC | 6.48 | 0.64% |
| EDA | 9.75 | 0.06% |
| TEMP | 11.27 | 0.68% |



### References

Gnana Subha, G., Suja Priyadharsini, S. An Efficient Algorithm Based on Combined Encoding Techniques for Compression of ECG Data from Multiple Leads. Wireless Pers Commun 108, 2137–2147 (2019). https://doi.org/10.1007/s11277-019-06513-9

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
