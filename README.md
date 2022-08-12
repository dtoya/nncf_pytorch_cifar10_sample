# nncf_pytorch_cifar10_sample

```
$ sudo apt graphviz-dev and graphviz
$ python3 -m venv venv
$ . venv/bin/activate
(venv) $ pip install -U pip
(venv) $ pip install -r requirements.txt
(venv) $ python cifar10_tutorial_nncf_finetune.py
```

Run MO and Benchmark_app on the environment having openvino-dev.
```
(openvino_env) $ mo --input_model model.onnx
(openvino_env) $ mo --input_model compressed_model.onnx
(openvino_env) $ benchmark_app -m model.xml
(openvino_env) $ benchmark_app -m compressed_model.xml
```


