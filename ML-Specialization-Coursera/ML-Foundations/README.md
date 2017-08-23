# Requested Resources: python v2.7 & GraphLab
The following note is the record of my install instruction.
For more information, please refer to the course introduction(W1).

## About download GraphLab Create
### https://turi.com/learn/coursera/

## Download Anacaonda2 and create env
conda create -n gl-env python=2.7 anaconda=4.0.0

## To activate the environment
source activate gl-env

## Install GraphLab Create
pip install --upgrade --no-cache-dir ___your-liscense-link-apply-from-graphlab___ GraphLab-CReate-License.tar.gz

## Install ipython-notebook
conda install ipython-notebook

### Every time you want to activate the env with GraphLab Create & SFrame
source activate gl-env

### If the SFrame crash, it may be because the liscense key config file corruption
try "sf = graphlab.SFrame()"
or, try "remove ~/.graphlab" and "graphlab.product_key.set_product_key()"
