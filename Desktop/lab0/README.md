# A Kernel Seedling
TODO: intro

## Building
```shell
make
```

## Running
```shell
sudo insmod proc_count.ko
cat /proc/count
```
This will load the module then output the contents of the /proc/count file, which is an integer indicating how many processes are running. 



## Removing module then cleaning Up
```shell
sudo rmmod proc_count
make clean
```

## Testing
```python
python -m unittest
```
Running the unit tests should display "OK" or "FAILED". It will cross check the loaded module with commands piped together to count the number of running processes. 
```shell
uname -r -s -v

```
Tested on Linux 5.14.8-arch1-1.
