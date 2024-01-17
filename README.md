# A Kernel Seedling
This is a skeleton for proc_count.c that returns an integer in /proc/count that is the number of running processes
on the machine. It makes use of the kernel

## Building
```shell
make
```

## Running
```shell
sudo insmod proc_count.ko
cat /proc/count
```
TODO: results?

## Cleaning Up
```shell
make clean
sudo rmmod proc_count
```

## Testing
```python
python -m unittest
```
...
----------------------------------------------------------------------
Ran 3 tests in 2.063s

OK

Report which kernel release version you tested your module on
(hint: use `uname`, check for options with `man uname`).
It should match release numbers as seen on https://www.kernel.org/.

```shell
uname -r -s -v
```
Linux 5.14.8-arch1-1 #1 SMP PREEMPT Sun, 26 Sep 2021 19:36:15 +0000