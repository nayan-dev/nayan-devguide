# Building Firmware

Fetch source code using following command:

```
git clone https://github.com/nayan-dev/Firmware
```

Update the submodules using following command after entering Firmware directory:

```
git submodule update --init --recursive
```

Compile firmware for master controller using `make nayan-mst_default` and upload by `make nayan-mst_default upload`

For slave controller do `make nayan-slv_default` for compile only and `make nayan-slv_default upload` to compile and upload.