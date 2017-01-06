TensorFlow
============
TensorFlow is an open source software library for numerical computation using
data flow graphs.  Nodes in the graph represent mathematical operations, while
the graph edges represent the multidimensional data arrays (tensors) that flow
between them.  This flexible architecture lets you deploy computation to one
or more CPUs or GPUs in a desktop, server, or mobile device without rewriting
code.  TensorFlow also includes TensorBoard, a data visualization toolkit.

## Invoking TensorFlow

TensorFlow is run simply by importing it as a Python module:

```
$ python
>>> import tensorflow as tf
>>> hello = tf.constant('Hello, TensorFlow!')
>>> sess = tf.Session()
>>> sess.run(hello)
Hello, TensorFlow!
>>> a = tf.constant(10)
>>> b = tf.constant(32)
>>> sess.run(a+b)
42
```

It will often be desirable to pull in data and model descriptions from
locations outside the container for use by TensorFlow.  To accomplish this, the
easiest method is to mount one or more host directories as [Docker data
volumes](https://docs.docker.com/engine/tutorials/dockervolumes/#/mount-a-host-directory-as-a-data-volume).

## Suggested Reading

Please refer to the TensorFlow website at https://www.tensorflow.org/get_started
for a tutorial and basic usage examples.

See `/workspace/README.md` inside the container as well as the following
websites for further information:

* [TensorFlow website](http://tensorflow.org)
* [TensorFlow whitepaper](http://download.tensorflow.org/paper/whitepaper2015.pdf)
* [TensorFlow Model Zoo](https://github.com/tensorflow/models)
* [TensorFlow MOOC on Udacity](https://www.udacity.com/course/deep-learning--ud730)
* [Community-authored resources](https://www.tensorflow.org/versions/master/resources#community)
