# TensorFlow Distribution Strategies

Last updated: Feb 08th 2022

**TODO: Add blog URL to here when it is up.**

This shows the `.ipynb` Jupyter notebooks from the TensorFlow tutorials [Distributed training with Keras](https://www.tensorflow.org/tutorials/distribute/keras) and [Custom training with tf.distribute.Strategy](https://www.tensorflow.org/tutorials/distribute/custom_training), slightly modified to run on Paperspace Gradient.

There is an associated blog entry for this repository.

## To run the notebooks

Assuming you are signed up for Paperspace and have access to multi-GPU machines (paid subscriptions include them), then:

- Create a project to put your Notebook instance in
- Create a Notebook with the following settings (the rest of the options can be left on default):
  - Container = TensorFlow 2.6.0 (Gradient recommended container)
  - Machine = multi-GPU, e.g., A5000x2
  - Workspace = https://github.com/gradient-ai/TensorFlow-Distribution-Strategies (this repository)
- Launch the Notebook

Once launched, the two Jupyter notebooks `keras.ipynb` and `custom_training.ipynb` should be visible in the files tab on the left-hand navigation bar. They can be opened and run.

- `keras.ipynb` shows a model on the MNIST dataset using a simple training loop
- `custom_training.ipynb` shows a more complicated setup on the Fashion-MNIST dataset using a custom training loop

*Note*: If you run several `.ipynb`s, you may get a GPU out-of-memory error since their allocated memory is not cleared. This can be remedied by restarting the Notebook instance.
