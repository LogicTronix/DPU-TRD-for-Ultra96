# DPU-TRD-for-Ultra96
This is DNNDK tutorial for ultra96 FPGA for implementing the DPU TRD design.


DPU TRD for Ultra96 FPGA [zcu100-revc]. This tutorial have implemented/build the "Resnet50" and "Face_Detection" targeting the Ultra96 FPGA. For developing the build we followed the "DPU Integration" tutorial at github of Xilinx.

Here is the downloadable file of the build, you can download and test it on Ultra96: https://drive.google.com/open?id=1k6Qx85yOmM3zNnACH_V_36utCF0KiOto

For testing on Ultra96 [reference: DPU integration tutorial: https://github.com/Xilinx/Edge-AI-Platform-Tutorials/tree/master/docs/DPU-Integration] , 
1. Copy the files from the above link into SD card [8GB or higher size]
2. Plug it to your Ultra96, Connect the JTAG-UART [or UART dongle] with ultra96
3. Connect the minidp display [monitor]
4. Connect the USB webcam [only needed for running the Face_detection application]
5. Press the power on Button,
6. Connect the Serial terminal at 115200 to the Ultra96 FPGA
7. you will get the running steps of ultra96 on serial terminal
8. now you can put login : root and password: root on terminal
9. enter:
export DISPLAY=:0.0
xrandr --output DP-1 --mode 800x600
xset -dpms
10. Change to the directory with the resnet50 application and execute the program. •	cd /media/card/resnet50 •	./resnet50.elf

11.hange to the following directories with the face_detection application and execute the program.

cd /media/card/face_detection
./face_detection.elf
Note: If you see “Open camera error!”, try unplugging the USB camera and inserting it again. If it still isn’t recognized, try rebooting with the camera unplugged, then plug in the camera before launching the application. If both of these efforts fail, try a different camera.



If you get any issues on testing this "demot-test-dpu-trd-ultra96" then write us an email, we will reply you within 24 hour. 
Mail: info@logictronix.com



Similar build is also available on "desktop-stretch" and "desktop-buster" for demo test provided by https://www.xilinx.com/products/design-tools/ai-inference/ai-developer-hub.html#edge

https://logictronix.com/our-resources/machine-learning-with-fpga/dpu-trd-for-ultra96/

#dnndk #neural #network #resnet50 #face_detection #dpu #trd #ultra96 #machine #learning
