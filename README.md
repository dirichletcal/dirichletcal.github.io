# Beyond temperature scaling: Obtaining well-calibrated multiclass probabilities with Dirichlet calibration

[Meelis Kull], [Miquel Perello Nieto], [Markus Kängsepp], [Telmo de Menezes e Silva Filho], [Hao Song], and [Peter Flach]

Class probabilities predicted by most multiclass classifiers are uncalibrated, often tending towards over-confidence. With neural networks, calibration can be improved by temperature scaling, a method to learn a single corrective multiplicative factor for inputs to the last softmax layer. On non-neural models the existing methods apply binary calibration in a pairwise or one-vs-rest fashion.

We propose a natively multiclass calibration method applicable to classifiers from any model class,
derived from Dirichlet distributions and generalising the beta calibration method from binary classification.
It is easily implemented with neural nets since it is equivalent to log-transforming the uncalibrated probabilities, followed by one linear layer and softmax.

Experiments demonstrate improved probabilistic predictions according to multiple measures (confidence-ECE, classwise-ECE, log-loss, Brier score) across a wide range of datasets and classifiers. Parameters of the learned Dirichlet calibration map provide insights to the biases in the uncalibrated model. 

## NeurIPS 2019

Click on the following links to access the paper or download the poster and the presentation slides from NeurIPS 2019.

* [NeurIPS2019 paper]
* [NeurIPS2019 poster] 
* [NeurIPS2019 slides]
* [NeurIPS2019 video] 
* [NeurIPS2019 experiments code] 

# Support or Contact

If you are having problems executing the experiments or the tutorials, do not hesitate to contact us.

[//]: # (References)
   [Meelis Kull]: <http://www.bris.ac.uk/engineering/people/meelis-kull/>
   [Miquel Perello Nieto]: <https://www.perellonieto.com/>
   [Markus Kängsepp]: <https://www.linkedin.com/in/markus-k%C3%A4ngsepp-10a95a142/?originalSubdomain=ee>
   [Telmo de Menezes e Silva Filho]: <https://www.researchgate.net/profile/Telmo_Silva_Filho>
   [Hao Song]: <http://www.bristol.ac.uk/engineering/people/hao-song/index.html>
   [Peter Flach]: <https://www.cs.bris.ac.uk/~flach/>
   [NeurIPS2019 paper]:  <https://github.com/dirichletcal/tobeadded>
   [NeurIPS2019 poster]: <https://dirichletcal.github.io/documents/neurips2019/poster.pdf>
   [NeurIPS2019 slides]: <https://dirichletcal.github.io/documents/neurips2019/slides.pdf>
   [NeurIPS2019 video]:  <https://dirichletcal.github.io/documents/neurips2019/video/>
   [NeurIPS2019 experiments code]:  <https://github.com/dirichletcal/experiments_neurips>
