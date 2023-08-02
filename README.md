# Secure Wireless Communication in MANETs using HC-12 Module

The purpose of this work is to generate and transmit text messages through a wireless communication system in a secure way. This facility prevails in the mobile network for which the user pays for it, whereas the system designed here can be used as a personal communication system and information can be transmitted free of cost. Moreover, the data is secured as it is encrypted at the transmitting end. To decrypt the  data at the receiver end, standard algorithms like **AES and RSA** are used. In our work, two- way communication system is implemented for transmitting the text information, wherein the sender can also act as a receiver and vice versa. The advantage of using this system is that the user can communicate the message over a long range.  The standard algorithms are used for both encryption and decryption purposes. These cryptographic algorithms which are used to protect information, are obtained from mathematical concepts to convert messages in ways that make it harder to decode them. The message entered through the keyboard by the sender is encrypted with the help of algorithms to generate an encrypted key (ciphertext). This ciphertext is transferred to HC-12 sender module which is then wirelessly transmitted to HC-12 receiver module. Once anything is typed on the serial monitor at the sender side, the same is reflected at the receiving end’s serial monitor. This message will be in the form of 16-bit for AES algorithm and 32-bit for RSA algorithm. In addition to personal communication, the system designed here can be used for applications like FASTag, automated parking, library management, etc. In our work, wireless communication is taking place through HC-12 module. The range is restricted to less than 600 meters and the range also depends upon factors such as line of sight, humidity, temperature, etc. But for long distances, a high power transmitter can be used.

Currently, numerous modules capable of wireless communication are available, but HC-12 is cost-effective and its excellent characteristics make this communication best suited for several embedded systems, and so on.

# HC-12 module
The HC-12 is a half-duplex wireless serial communication module with 100 channels in the 433.4-473.0 MHz range that is capable of transmitting up to 1 km.
HC-12 wireless serial port communication module is a new-generation multichannel embedded wireless data transmission module. Its wireless working frequency band is 433.4-473.0MHz, multiple channels can be set, with the stepping of 400 KHz, and there are total of 100 channels. The maximum transmitting power of the module is 100mW (20dBm), the receiving sensitivity is -117dBm at a baud rate of 5,000bps in the air, and the communication distance is 1,000m in open space. The module is encapsulated with a stamp hole, can adopt patch welding, and its dimension is 27.8mm × 14.4mm × 4mm (including antenna cap, excluding spring antenna), so it is very convenient for customers to go into the application system. There is a PCB antenna pedestal ANT1 on the module, and the user can use the external antenna of 433M frequency band through coaxial cable; there is also an antenna solder eye ANT2 in the module, and it is convenient for user to weld spring antenna. Users could select one of these antennas according to use requirements. There is MCU inside the module, and the user doesn’t need to program the module separately, and all transparent transmission mode is only responsible for receiving and sending serial port data, so it is convenient to use. 

[image](https://github.com/vishwas98/AES_RSA-Using-Arduino_Uno/assets/39726573/f116861a-c305-4e92-8279-2c5fdb120a67)

# LoRa : Long-Range Radio
LoRa enables long-range transmissions (more than 10 km in rural areas) with low power consumption. The technology covers the physical layer, while other technologies and protocols such as LoRaWAN (Long Range Wide Area Network) cover the upper layers. LoRa devices and the open LoRaWAN protocol enable smart IoT applications that solve some of the biggest challenges facing our planet: energy management, natural resource reduction, pollution control, infrastructure efficiency, disaster prevention, and more.

# Cryptography
Cryptography is a technique of securing information and communications through the use of codes so that only those people for whom the information is intended can understand it and process it. Thus, preventing unauthorized access to information. In Cryptography, the techniques which are used to protect information are obtained from mathematical concepts and a set of rule-based calculations known as algorithms to convert messages in ways that make it hard to decode them. These algorithms are used for cryptographic key generation, digital signing, verification to protect data privacy, web browsing on the internet and to protect confidential transactions such as credit card and debit card transactions.

# Arduino IDE
The Arduino Integrated Development Environment (IDE) is a cross-platform application (for Windows, macOS, Linux) that is written in functions from C and C++. It is used to write and upload programs to Arduino-compatible boards, but also, with the help of 3rd party cores, other vendor development boards. The source code for the IDE is released under the GNU General Public License, version 2. The Arduino IDE supports the languages C and C++ using special rules of code structuring. The Arduino IDE supplies a software library from the Wiring project, which provides many common input and output procedures. User-written code only requires two basic functions, for starting the sketch and the main program loop, that is compiled and linked with a program stub main() into an executable cyclic executive program with the GNU toolchain, also included with the IDE distribution. The Arduino IDE employs the program avrdude to convert the executable code into a text file in hexadecimal encoding that is loaded into the Arduino board by a loader program in the board's firmware. By default, avrdude is used as the uploading tool to flash the user code onto official Arduino boards. With the rising popularity of Arduino as a software platform, other vendors started to implement custom open-source compilers & tools (cores) that can build and upload sketches to other MCUs that are not supported by Arduino's official line of MCUs. In October 2019 the Arduino organization began providing early access to a new Arduino Pro IDE with debugging and other advanced features. The website to download Arduino IDE https://www.arduino.cc/en/Main/Software

[image](https://github.com/vishwas98/AES_RSA-Using-Arduino_Uno/assets/39726573/66945aea-2226-46d8-9634-677125eca2e6)


# Arduino Uno
Arduino Uno is a microcontroller board based on the ATmega328P (datasheet). It has 14 digital input/output pins, 6 analog inputs, a 16 MHz ceramic resonator (CSTCE16M0V53-R0), a USB connection, a power jack, an ICSP header and a reset button. It contains everything needed to support the microcontroller; simply connect it to  a computer with a USB cable or power it with an AC-to-DC adapter or battery to get started.

[image](https://github.com/vishwas98/AES_RSA-Using-Arduino_Uno/assets/39726573/3c95f428-6609-4f3c-9c39-dffd0d8ca006)


# Proposed Algorithm
The more popular and widely adopted symmetric encryption algorithm is the Advanced Encryption Standard (AES). It is found that AES is much faster than RSA.

The features of AES are as follows -
•	Symmetric algorithm that requires only one encryption and decryption key
•	Easy overall implementation
•	Stronger and faster than RSA
•	Provide full specification and design details
•	Software implementable in C and Java languages

Another widely used cryptographic algorithm for secure data transmission is Rivest- Shamir-Adleman (RSA). It is an asymmetric cryptographic algorithm. Asymmetric means that there are two different keys. This is also called public key cryptography, because one of the keys can be given to anyone.

The features of RSA are as follows -
•	Popular exponentiation in a finite field over integers including prime numbers.
•	The integers used by this method are sufficiently large making it difficult to solve.
•	There are two sets of keys in this algorithm: private key and public key.

# Flow Chart
The below figures show the developed flow chart of the message generated and the received:

[image](https://github.com/vishwas98/AES_RSA-Using-Arduino_Uno/assets/39726573/675f3a96-7217-4798-822c-68f3b4007c20)


[image](https://github.com/vishwas98/AES_RSA-Using-Arduino_Uno/assets/39726573/983088e9-591b-4a26-8593-ec143a4de85d)
# System Design
The block diagram of wireless communication using Arduino integrated with HC-12 is as shown below:

[image](https://github.com/vishwas98/AES_RSA-Using-Arduino_Uno/assets/39726573/19419dd7-4602-4b3f-9b23-47246136c1b0)

Initially, the Arduino and HC12 components are connected to the respective sender and receiver system. The circuit schematic is as shown in figure 5. The operating voltage of the module is from 3.2 V to 5.5 V. In this work, PC USB is used as a power to the components. Since the developed work is a two-way communication system, the same code is used for both Arduino. Arduino HC12 setup can either be made on two separate computers or a single computer. Arduino IDE is an open-source software that can be used to write the code and upload it on the Arduino component. A serial monitor is used for transmitting and receiving messages.

# Circuit Diagram of Proposed Model
[image](https://github.com/vishwas98/AES_RSA-Using-Arduino_Uno/assets/39726573/4977f805-c523-4abc-a137-c9b162f18e65)

# Working
Enter the data to be sent

[image](https://github.com/vishwas98/AES_RSA-Using-Arduino_Uno/assets/39726573/da44ac1b-2c2a-4798-bfd1-2e54b4b67bb8)


Entered 16-bit data

[image](https://github.com/vishwas98/AES_RSA-Using-Arduino_Uno/assets/39726573/d2cdde30-d107-433d-a8c5-1689147149da)


At sender side, the original message is entered. The AES or RSA algorithm is used to encrypt the message. After the encryption, the encrypted message is displayed and sent to receiver with the help of HC-12 module.

[image](https://github.com/vishwas98/AES_RSA-Using-Arduino_Uno/assets/39726573/e46cf9ae-5fab-4b69-83c4-29f2ccc1e478)

At the receiver side, encrypted message which was sent by the sender gets decrypted using AES or DES algorithm and the original message is displayed on the serial monitor as shown in the figure

[image](https://github.com/vishwas98/AES_RSA-Using-Arduino_Uno/assets/39726573/257195aa-e8b7-473e-a8c1-83328d54d130)



# Sender side Analysis
At sender side, original message that needs to be transmitted is entered on serial monitor of the sender. AES or RSA algorithms are used to encrypt the original message into a form, where attackers fail to distinguish the original message. After the encryption, encrypted message is sent to the receiver system. The figure 9.1 shows the sender side transmission.



# Reciever side Analysis
At the receiver side, encrypted message is received. This encrypted message gets displayed on serial monitor of the receiver. Algorithms like AES or RSA take encrypted message as input and decrypt it in order to get back the original message. The original message gets displayed on the serial monitor of the receiver. The figure shows the receiver side reception.

# Analysis between AES and RSA
The most important aspect of day to day life is security. We have come up with this project to ensure that the data to be transmitted in least amount of time and in secure manner. Comparative analysis is made between two standard algorithms namely AES and RSA. So, for enhancing security, a comparative analysis along with various parameters for both the symmetric key encryption and asymmetric key encryption is presented. Parameters that need to be considered are number of characters, distance and time taken to send the message to the receiver. 

Below table is the analysis that we have made with varying distances and number of characters.

Distance : 40 meters 

[40meters]![image](https://github.com/vishwas98/AES_RSA-Using-Arduino_Uno/assets/39726573/c8f92b34-891a-4ac3-ab9a-2b58f34bca53)


Distance : 100 meters 

![100meters]![image](https://github.com/vishwas98/AES_RSA-Using-Arduino_Uno/assets/39726573/08e07b55-dd2b-4351-b91f-9d677a51b6c6)


Distance : 200 meters 

[200meters]![image](https://github.com/vishwas98/AES_RSA-Using-Arduino_Uno/assets/39726573/a790bd36-50dd-407e-85f9-68c07daee6e7)


Distance : 400 meters 

[400meters]![image](https://github.com/vishwas98/AES_RSA-Using-Arduino_Uno/assets/39726573/888ddb0a-aa92-472e-8770-8b5e16bafc03)


# Conclusion
In this work, an authenticated user can able to send and receive the message, thus eliminating the security issue. This two-way communication system restricts unauthorized access to the messages that is taking place between two nodes. Companies and government sectors can use this system to communicate between their employees. Agriculture sectors can also use this work in order to maintain relations with their buyers. In this project, a detailed comparison is made between two standard algorithms, namely AES and RSA. The system is designed as user friendly and its operation is quite simple.

We have found that RSA solves the problem of key agreement and key exchange generated in private-key cryptography algorithms but still, there is lack of confidentiality. AES is a private key-based algorithm that suffers from key distribution and key  agreement problems. However, the problem is solved in RSA algorithm but encryption and decryption take more time in RSA. Therefore, both algorithms have their own merits and demerits. Based on the computation time, AES is faster compared to RSA. AES took an average of 4 seconds to transmit 8-bit message to the receiver, whereas RSA took 6 seconds to transmit 8-bit message.

# Future Scope
Additional features can be incorporated into this system if required. Since this project is limited to a 1 km range due to use of the HC12 module, long-distance communication can also be implemented if we use more sophisticated modules like LoRa which has  a range of more than 10 km. The length of the message to be transmitted can also be increased by modifying the micro-controller program. This project is restricted to text message transmission. We can further incorporate type of message like images, files and so on. To ensure high security, Elliptic Curve Digital Signature Algorithm (ECDSA) can be  used as a substitute of RSA algorithm module.
