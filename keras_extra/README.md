# �����Keras����½��ж�GPU����

keras��Ҫʹ��tensorflow��Ϊbackend

���ñ��ļ���`keras_extra.py��`��`make_parallel`����

```
# use it like follows
model=Model(inputs=inputs,outputs=outputs)
model=make_parallel(model,2)  # this line is important
model.compile(optimizer='adadelta',loss='categorical_crossentropy',metrics=['accuracy'],)
```

The solution is according to https://medium.com/@kuza55/transparent-multi-gpu-training-on-tensorflow-with-keras-8b0016fd9012