# Hw7
## How to run program

Add a new empty Mbed program

Replace main.cpp with the main.cpp in the repository

Add the file arm_fir_data.c to the project

Add library mbed dsp to the project

https://os.mbed.com/teams/mbed-official/code/mbed-dsp

Add a #define to the file arm_bitreversal2.S

## Verification by matlab

copy input and output data (test data and gyro data) from STM board and paste it in a .txt file

use verification.m to verify if the CMSIS FIR function work or not

verification.m will first demonstrate if the higer signal in test data (combined sine wave) can be successfully filtered and compare it with the data processed by matlab's FIR filter

then compare the gyro data processed by matlab's FIR filter and CMSIS function

## Results
### Verify the program with a test signal

![inputs_and_outputs_of_test_data](https://user-images.githubusercontent.com/59012686/234929148-1d09d3f6-911d-463c-b7ac-33f628f69d8c.jpg)

### Compare the test result processed by matlab FIR filter and CMSIS FIR function

![compare_low_pass_filter_by_input_data](https://user-images.githubusercontent.com/59012686/234928217-1735ad72-1f8e-42b6-ab59-158ba9e65cdc.jpg)

### Compare gyro data result processed by matlab FIR filter and CMSIS FIR function

![compare_low_pass_filter_by_gyro_data](https://user-images.githubusercontent.com/59012686/234929134-6016846f-37b0-4198-8442-9981b8f224d3.jpg)
