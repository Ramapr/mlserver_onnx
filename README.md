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

1. copy directory
```
$ cp /onnx mlserver/runtimes
```
2. update [Dockerfile](https://github.com/SeldonIO/MLServer/blob/master/Dockerfile#L8)
```bash
COPY ../onnx ./runtimes/onnx
```
3. insert in [pyproject.toml](https://github.com/SeldonIO/MLServer/blob/master/pyproject.toml#L114)
```
mlserver-onnx = {path = "./runtimes/onnx", develop = true}
```
4. update poetry https://github.com/SeldonIO/MLServer/blob/master/poetry.lock 
