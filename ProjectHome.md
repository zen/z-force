# Hacking Z-Wave Home Automation Systems #

Presented by Behrang Fouladi and Sahand Ghanoun at [BlackHat USA 2013](https://www.blackhat.com/us-13/briefings.html#Fouladi)

Home automation systems provide a centralized control and monitoring function for heating, ventilation and air conditioning (HVAC), lighting and physical security systems. The central control panel and various household devices such as security sensors and alarm systems are connected with each other to form a mesh network over wireless or wired communication links and act as a "smart home". Zigbee and Z-wave wireless communication protocols are the most common used RF technology in home automation systems. Zigbee is based on an open specification and has been the subject of several academic and practical security researches. Z-wave is a proprietary wireless protocol that works in the Industrial, Scientific and Medical (ISM) radio band. Unlike Zigbee, no public security research on Z-Wave protocol was available before our work.

During this talk, we presented our analysis of the Z-Wave protocol stack layers including the security layer as well as our Z-Wave packet interception and injection tool **(Z-Force)**. Using this tool, we identified a critical implementation vulnerability in Z-Wave security layer and demonstrated a remote attack to comrpomise an AES encrypted Z-Wave door lock.

Our [presentation slides](http://drive.google.com/uc?export=view&id=0B8l07E7STihRVndmRmNfS1lGdlk&nonsesnse=something.pdf) are available on the project website. Detailed analysis of Z-Wave security layer and vulnerability description could be found in our [research paper](http://drive.google.com/uc?export=view&id=0B8l07E7STihRTDB3WmEza1ludEk&nonsesnse=something.pdf).

The public version of the **Z-Force** tool and radio firmware files are made available via [Z-Force project on Google Code](http://code.google.com/p/z-force/).