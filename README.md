# Executable data analyser static test project
This program is able to read data `.csv` from the datafile capted by the test and make graph automatically, saving the graph photo with its informations like force, thrust, maximum force, etc..

## All data is capted by a instrumentation system

The instrumentation system is composed by:

1. Arduino UNO; 
2. HX711;
3. Load Cell. 

![](./schematic.jpg)

Also, in the `.ino` file can be seen that the code can capture more data in addition to the force data, however, the system is not complete to do so. It requires sensor implementation. Nevertheless, the code is ready to be tested when the hardware be implemented.


[Tutorial video [PT-BR]](https://www.youtube.com/watch?v=GXkCo5zUSEQ&t=8s&ab_channel=RenanLarrieu)

## According to the tutorial, the process generates files as shown below

### 1. Graph `.png` [file](Plot_test1.png)

![](./Plot_test1.png)

### 2. Data `.txt` [file](data_test.txt)

![](./print_data_txt.png)

## HX711 use specifications

1. In the case of [`dados_teste_1.csv`](dados_teste_1.csv) all the data were capted at 10Hz frequency.

2. But, as can be seen, the frequency can be adjusted to 80Hz, however it also increase the noise.

![](./output_data_rate.png)

3. The communication protocol used by the device is I2C