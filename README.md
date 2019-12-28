# Detecting Sockpuppets in Deceptive Opinion Spam
Authors : **Marjan Hosseinia** and **Arjun Mukherjee** [\[preprint pdf\]](https://arxiv.org/pdf/1703.03149.pdf) [\[Springer pdf\]](https://link.springer.com/chapter/10.1007/978-3-319-77116-8_19)

We  explore  the  problem  of  sockpuppet  detection in deceptive opinion spam using authorship attribution and verification approaches. Two methods are explored. The first is a feature subsam-pling scheme that uses the KL-Divergence on stylistic language models of an author to find discriminative features. The second is a transduction scheme, spy induction that leverages the diversity of authors in theunlabeled test set by sending a set of spies (positive samples) from train-ing set to retrieve hidden samples in the unlabeled test set using nearest and farthest neighbors. Experiments using ground truth sockpuppet data show the effectiveness of the proposed schemes


# Spy-Induction Algorithm
For the problems which suffers from lack of training data, spy-induction algorithm improve training. It has three main steps:
First is spy selection where some carefully selected positive samples are sent to the unlabeled test set. The second step is to find certain Nearest and Farthest Neighbors (abbreviated NN,FN  henceforth)  of  the  positive  spy  samples  in  the  unlabeled  test  set.  As  the instances retain their original identity, a good distance metric should be able to retrieve potentially hidden positive (using common NN across different positive spies) and negative (using common FN across different positive spies) samples in the unlabeled test set. These newly retrieved samples from unlabeled test set are used to grow the training set. 

![spy-incuction](https://github.com/marjanhs/sockpuppet/blob/master/spy_induction.png)





Please contact me (![email:](https://raw.githubusercontent.com/marjanhs/stance/master/email.png)) to request the dataset!
