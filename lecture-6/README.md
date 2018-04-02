DEBUGGING CONVOLUTIONAL NEURAL NETWORKS
=======================================

# Downloading requirements

In order to run the experiments in this folder you will need to clone the tensorflow models repository from `https://github.com/tensorflow/models`. For instance to download using ssh:

    git clone git@github.com:tensorflow/models.git

You will also need to download a pre-trained checkpoint of inception resnet version2. You can do so from https://github.com/tensorflow/models/tree/master/research/slim#pre-trained-models For instance:

    wget http://download.tensorflow.org/models/inception_resnet_v2_2016_08_30.tar.gz

After you download the archive, extract it:

    tar -xzvf inception_resnet_v2_2016_08_30.tar.gz

# Install required packages

Using your favorite python environment manager(e.g. conda or venv) install the python package requirements:

    pip install -r requirements.txt

NOTE: the default configuration will install regular tensorflow(non-gpu) if you have configured GPU, better install tensorflow-gpu==1.5.0

# Configuring the notebooks

Each of the two notebooks has a cell with constants at the top where you can configure the paths to the location where you checked out tensorflow/models and where you extracted the inception resnet v2 checkpoint. By default those are assumed to be in the project root folder. If you decided to use a different location you need to update those locations.

