https://micropython.org/download/

1. Install python
2. Upgrade pip
```cmd
> python.exe -m pip install --upgrade pip
```
3. Install esptool
```cmd
> pip install esptool
```
4. Download appropritae firmware from https://micropython.org/download/
5.
```
> esptool.py --chip esp32 --port COM3 erase_flash
> esptool.py --chip esp32 --port COM3 --baud 460800 write_flash -z 0x1000 esp32-20190125-v1.10.bin
```
