## tft-explore

Playing around with Tensorflow Transform for making input pipelines

A few notes:
* Can only use TFT in Python 2.7!  Per [this](https://github.com/tensorflow/transform/issues/1) and [this](https://issues.apache.org/jira/browse/BEAM-1373), waiting on Python 3 support for `apache-beam`
* Per [this](https://github.com/andrix/python-snappy/pull/59/commits), you may need to run `sudo apt-get install libsnappy-dev` before installing `python-snappy`

===

While I have found TFT super-useful, I am still constrained by preprocessing that can be done with native TF ops since TFT exports a TF Graph.  I haven't found ways to do common text preprocessing steps, e.g. lowercase, Porter stemming, removing stop words, with TF/TFT.
