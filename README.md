<div align="center">
  <img src="https://www.tensorflow.org/images/tf_logo_transp.png"><br><br>
</div>

-----------------


| **`Documentation`** |
|-----------------|
| [![Documentation](https://img.shields.io/badge/api-reference-blue.svg)](https://www.tensorflow.org/api_docs/) |

**TensorFlow** 是一个使用数据流图进行数值计算的开源软件库。图形节点表示数学运算，而图形边缘表示在它们之间流动的多维数据阵列（张量）。这种灵活的体系结构使您可以将计算部署到桌面，服务器或移动设备中的一个或多个CPU或GPU，而无需重写代码。TensorFlow还包括[TensorBoard](https://www.tensorflow.org/guide/summaries_and_tensorboard), 一种数据可视化工具包。

TensorFlow 最初是由研究人员和工程师在Google机器智能研究组织的Google Brain团队开发的，目的是进行机器学习和深度神经网络研究。该系统通用性足以适用于各种其他领域。

TensorFlow提供稳定的Python API和C API，以及没有API向后兼容性保证，如C ++，Go，Java，JavaScript和Swift。
通过订阅[announce@tensorflow.org](https://groups.google.com/a/tensorflow.org/forum/#!forum/announce)了解发布公告和安全更新的最新信息 。

## 安装
*有关如何安装发行二进制文件或如何从源构建的说明，请参阅安装 [Installing TensorFlow](https://www.tensorflow.org/get_started/os_setup.html)*

喜欢冒险的人也可以尝试我们的夜间二进制文件：

**Nightly pip packages**
* 我们很高兴地宣布，TensorFlow现在在pypi 的[tf-nightly](https://pypi.python.org/pypi/tf-nightly) 和
[tf-nightly-gpu](https://pypi.python.org/pypi/tf-nightly-gpu) 项目下提供夜间点包。只需运行`pip install tf-nightly`或`pip install tf-nightly-gpu`在干净的环境中安装TensorFlow构建。我们支持Linux，Mac和Windows上的CPU和GPU包。


#### *试试你的第一个TensorFlow程序*
```shell
$ python
```
```python
>>> import tensorflow as tf
>>> hello = tf.constant('Hello, TensorFlow!')
>>> sess = tf.Session()
>>> sess.run(hello)
'Hello, TensorFlow!'
>>> a = tf.constant(10)
>>> b = tf.constant(32)
>>> sess.run(a + b)
42
>>> sess.close()
```
在[tensorflow.org](https://www.tensorflow.org/tutorials/)教程页面中了解有关如何在TensorFlow中执行特定任务的更多示例.

## 贡献指南

**如果您想为TensorFlow做出贡献，请务必查看[贡献指南](CONTRIBUTING.md). 该项目遵守TensorFlow的
[行为准则](CODE_OF_CONDUCT.md). 通过参与，您应该支持此代码。**

**我们使用 [GitHub issues](https://github.com/tensorflow/tensorflow/issues) 来跟踪请求和错误. 所以请参阅
[TensorFlow 社区](https://groups.google.com/a/tensorflow.org/forum/#!forum/discuss) 一般问题和讨论，并请将具体问题直接发送到 [Stack Overflow](https://stackoverflow.com/questions/tagged/tensorflow).**

TensorFlow项目致力于遵循开源软件开发中普遍接受的最佳实践：

[![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/1486/badge)](https://bestpractices.coreinfrastructure.org/projects/1486)


## Continuous build status

### Official Builds

| Build Type      | Status | Artifacts |
| ---             | ---    | ---       |
| **Linux CPU**   | [![Status](https://storage.googleapis.com/tensorflow-kokoro-build-badges/ubuntu-cc.svg)](https://storage.googleapis.com/tensorflow-kokoro-build-badges/ubuntu-cc.html) | [pypi](https://pypi.org/project/tf-nightly/) |
| **Linux GPU**   | [![Status](https://storage.googleapis.com/tensorflow-kokoro-build-badges/ubuntu-gpu-py3.svg)](https://storage.googleapis.com/tensorflow-kokoro-build-badges/ubuntu-gpu-py3.html) | [pypi](https://pypi.org/project/tf-nightly-gpu/) |
| **Linux XLA**   | [![Status](https://storage.googleapis.com/tensorflow-kokoro-build-badges/ubuntu-xla.svg)](https://storage.googleapis.com/tensorflow-kokoro-build-badges/ubuntu-xla.html) | TBA |
| **MacOS**       | [![Status](https://storage.googleapis.com/tensorflow-kokoro-build-badges/macos-py2-cc.svg)](https://storage.googleapis.com/tensorflow-kokoro-build-badges/macos-py2-cc.html) | [pypi](https://pypi.org/project/tf-nightly/) |
| **Windows CPU** | [![Status](https://storage.googleapis.com/tensorflow-kokoro-build-badges/windows-cpu.svg)](https://storage.googleapis.com/tensorflow-kokoro-build-badges/windows-cpu.html) | [pypi](https://pypi.org/project/tf-nightly/) |
| **Windows GPU** | [![Status](https://storage.googleapis.com/tensorflow-kokoro-build-badges/windows-gpu.svg)](https://storage.googleapis.com/tensorflow-kokoro-build-badges/windows-gpu.html) | [pypi](https://pypi.org/project/tf-nightly-gpu/) |
| **Android**     | [![Status](https://storage.googleapis.com/tensorflow-kokoro-build-badges/android.svg)](https://storage.googleapis.com/tensorflow-kokoro-build-badges/android.html) | [![Download](https://api.bintray.com/packages/google/tensorflow/tensorflow/images/download.svg)](https://bintray.com/google/tensorflow/tensorflow/_latestVersion) |


### Community Supported Builds

| Build Type      | Status | Artifacts |
| ---             | ---    | ---       |
| **IBM s390x**       | [![Build Status](http://ibmz-ci.osuosl.org/job/TensorFlow_IBMZ_CI/badge/icon)](http://ibmz-ci.osuosl.org/job/TensorFlow_IBMZ_CI/) | TBA |
| **IBM ppc64le CPU** | [![Build Status](http://powerci.osuosl.org/job/TensorFlow_Ubuntu_16.04_CPU/badge/icon)](http://powerci.osuosl.org/job/TensorFlow_Ubuntu_16.04_CPU/) | TBA |
| **IBM ppc64le GPU** | [![Build Status](http://powerci.osuosl.org/job/TensorFlow_Ubuntu_16.04_PPC64LE_GPU/badge/icon)](http://powerci.osuosl.org/job/TensorFlow_Ubuntu_16.04_PPC64LE_GPU/) | TBA |
| **Linux CPU with Intel® MKL-DNN** Nightly | [![Build Status](https://tensorflow-ci.intel.com/job/tensorflow-mkl-linux-cpu/badge/icon)](https://tensorflow-ci.intel.com/job/tensorflow-mkl-linux-cpu/) | [Nightly](https://tensorflow-ci.intel.com/job/tensorflow-mkl-build-whl-nightly/) |
| **Linux CPU with Intel® MKL-DNN** Python 2.7<br> **Linux CPU with Intel® MKL-DNN** Python 3.5<br>  **Linux CPU with Intel® MKL-DNN** Python 3.6 | [![Build Status](https://tensorflow-ci.intel.com/job/tensorflow-mkl-build-release-whl/badge/icon)](https://tensorflow-ci.intel.com/job/tensorflow-mkl-build-release-whl/lastStableBuild)|[1.9.0 py2.7](https://storage.googleapis.com/intel-optimized-tensorflow/tensorflow-1.9.0-cp27-cp27mu-linux_x86_64.whl)<br>[1.9.0 py3.5](https://storage.googleapis.com/intel-optimized-tensorflow/tensorflow-1.9.0-cp35-cp35m-linux_x86_64.whl)<br>[1.9.0 py3.6](https://storage.googleapis.com/intel-optimized-tensorflow/tensorflow-1.9.0-cp36-cp36m-linux_x86_64.whl) |


## For more information
* [Tensorflow Blog](https://medium.com/tensorflow)
* [TensorFlow Course at Stanford](https://web.stanford.edu/class/cs20si)
* [TensorFlow Model Zoo](https://github.com/tensorflow/models)
* [TensorFlow MOOC on Udacity](https://www.udacity.com/course/deep-learning--ud730)
* [TensorFlow Roadmap](https://www.tensorflow.org/community/roadmap)
* [Tensorflow Twitter](https://twitter.com/tensorflow)
* [TensorFlow Website](https://www.tensorflow.org)
* [TensorFlow White Papers](https://www.tensorflow.org/about/bib)
* [TensorFlow YouTube Channel](https://www.youtube.com/channel/UC0rqucBdTuFTjJiefW5t-IQ)

Learn more about the TensorFlow community at the [community page of tensorflow.org](https://www.tensorflow.org/community) for a few ways to participate.

## License

[Apache License 2.0](LICENSE)
