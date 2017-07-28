#Testing the arduino is connected

install package to allow us to compile arduino code to /usr/share/arduino
```
sudo apt-get install arduino-core arduino-mk
```

add user to dialout group to allow us to upload code to the arduino board
```
sudo usermod -a -G dialout pi
```


build and upload the file to arduino
```
make
make upload
```


run python file to test that we're receiving signals from the arduino board
```
./test.py
```
