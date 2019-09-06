### Last Updated September 2019

## There may be some issues that aren’t covered in this quick guide and will be updated in the future.

# URSim and URCap Installation Guide on Ubuntu – No Virtual Machine Necessary 

This guide goes over how to Install URSim natively to Ubuntu 18.04 systems.

Steps to install

1. Open a terminal and install Maven ```sudo apt install maven```, Java8 ```sudo apt install openjdk-8-jdk``` (you may need to install other dependencies as well

2. Set Java version to Java 8 ```sudo update-alternatives --config java``` and select java 8

3. Download [URCap SDK](https://plus.universal-robots.com/download-center/urcaps-sdk/) and [URSim](https://www.universal-robots.com/download/) from the UR Website

4. Extract both packages to your Home directory

5. Navigate to /home/username/ursim/ursim-XXXX and open a terminal. Run ```./install.sh```

6. Navigate to /home/username/sdk-1.7.0 and open a terminal. Run ```./install.sh```

7. To run navigate back to the Ursim directory /home/username/ursim/ursim-XXXX and open terminal and run ```./start-ursim.sh```

Compiling URCap Project

1. Navigate to your pom.xml file for your maven/urcap project and open

2. Make sure the ‘Install path for the UR Sim’ matches were your Ursim folder location and name.

3. Navigate to your URCap folder and run ```mvn install -P ursim```

4. Run URSim