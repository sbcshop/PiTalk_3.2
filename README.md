
# PiTalk_3.2

Modular Smartphone on Raspberry Pi.

<img src="Icons/pitalk.png" width="300"><img src="http://pitalk.co.uk/img/h11.png" width="300">

**Steps for PiTalk software installation -** 

1. Open Terminal and download the code by writing: 
   ```
   git clone https://github.com/sbcshop/PiTalk_3.2.git
   ```

2. Your code will be downloaded to '/home/pi' directory. Use 'ls' command to check the list of directories.

3. Go to directory 'PiTalk_3.2' and run the command to change the permissions:
   ```
   sudo chmod +x setup
   ```
   and then run 'setup', but make sure Raspberry Pi is connected to Internet.
   ```
   sudo ./setup
   ```
   It will reboot your Raspberry Pi

4. Go to directoy 'PiTalk_3.2' and you will see there are two GUI files i.e. GUI32_Landscape.py and GUI32_Portrait.py. As its name indicates    it will create PiTalk GUI in Landscape and Portrait mode.

5. Lets run the PiTalk code (Landscape or Portrait Mode). Open the terminal and write:

   For Raspberry Pi 3 or 3B+ use 'ttyS0' if PiTalk is connected through GPIO or 'ttyUSB3' if connected through USB
   ```
   sudo python3 ./GUI32_Landscape.py ttyS0
   ```
   For other version use 'ttyAMA0' if connected through GPIO or 'ttyUSB3' if connected throught USB
   or 
   ```
   sudo python3 ./GUI32_Portrait.py ttyAMA0
   ```
   **Note**: Default it will take 'ttyS0' port. It means if you simply write :
   ```
   sudo python3 ./GUI32_Portrait.py
   ```
   or 
   ```
   sudo python3 ./GUI32_Landscape.py
   ```
   It will also work but for Raspberry Pi 3 or 3B+ only.
   
6. It will run PiTalk code on HDMI screen. If you want to run this code on 3.2" LCD, go to 'setting' app and go to 'Screen
   Orientation'. You will see diffrent orientation at different angles. Click to any angle will reboot your Raspberry Pi and start GUI
   on 3.2" LCD.
   
7. Now to run the PiTalk code on 3.2" LCD, repeat **Step 5** 


For more details, go to http://pitalk.co.uk/

For blogs and projects, go to http://sb-components.co.uk/pitalk-blog.html

Go to https://shop.sb-components.co.uk/ to order your PiTalk now
