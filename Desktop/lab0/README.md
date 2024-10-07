# A Kernel Seedling
TODO: intro

## Building
```shell
make
```

## Running
```shell
sudo insmod proc_count.ko
```
cat /proc/count

## Cleaning Up
```shell
make clean
```

## Testing
```python
python -m unittest
```
Result should be an integer indicating how many processes are running.

```shell
uname -r -s -v

```
Tested on Linux 5.14.8-arch1-1.
