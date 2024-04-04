# mlserver_onnx
The mlserver extension is used to run model in onnx format.
[mlserver doc](https://mlserver.readthedocs.io/en/latest/getting-started/index.html)

# struct 

```
onnx/mlseerver_onnx/...
 |
  __init__.py
  onnx.py
```
place to 

# how to build 

[Dockerfile](https://github.com/SeldonIO/MLServer/blob/master/Dockerfile)

go to [runtimes](https://github.com/SeldonIO/MLServer/blob/master/Dockerfile#L8)

```
COPY ../onnx ./runtimes/onnx
```
update poetry https://github.com/SeldonIO/MLServer/blob/master/poetry.lock 
