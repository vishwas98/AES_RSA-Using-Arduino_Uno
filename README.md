

# Sender side Analysis
At sender side, original message that needs to be transmitted is entered on serial monitor of the sender. AES or RSA algorithms are used to encrypt the original message into a form, where attackers fail to distinguish the original message. After the encryption, encrypted message is sent to the receiver system. The figure 9.1 shows the sender side transmission.

# Reciever side Analysis
At receiver side, encrypted message is received. This encrypted message gets displayed on serial monitor of the receiver. Algorithms like AES or RSA take encrypted message as input and decrypt it in order to get back the original message. Original message gets displayed on the serial monitor of the receiver. The figure shows the receiver side reception.

# Analysis between AES and RSA
The most important aspect of day to day life is security. We have come up with this project to ensure that the data to be transmitted in least amount of time and in secure manner. Comparative analysis is made between two standard algorithms namely AES and RSA. So, for enhancing the security, a comparative analysis along with various parameters for both the symmetric key encryption and asymmetric key encryption is presented. Parameters that need to be considered are number of characters, distance and time taken to send the message to the receiver. 

Below table is the analysis that we have made with varying distances and number of characters.

Distance : 40 meters 

![40meters][image](https://github.com/vishwas98/AES_RSA-Using-Arduino_Uno/assets/39726573/c8f92b34-891a-4ac3-ab9a-2b58f34bca53)


Distance : 100 meters 

![100meters][image](https://github.com/vishwas98/AES_RSA-Using-Arduino_Uno/assets/39726573/08e07b55-dd2b-4351-b91f-9d677a51b6c6)


Distance : 200 meters 

![200meters][image](https://github.com/vishwas98/AES_RSA-Using-Arduino_Uno/assets/39726573/a790bd36-50dd-407e-85f9-68c07daee6e7)


Distance : 400 meters 

![400meters][image](https://github.com/vishwas98/AES_RSA-Using-Arduino_Uno/assets/39726573/888ddb0a-aa92-472e-8770-8b5e16bafc03)


# Conclusion
In this work, an authenticated user can able to send and receive the message, thus eliminating the security issue. This two-way communication system restricts unauthorized access to the messages that is taking place between two nodes. Companies and government sectors can use this system to communicate between their employees. Agriculture sectors can also use this work in order to maintain relations with their buyers. In this project, a detailed comparison is made between two standard algorithms, namely AES and RSA. The system is designed as user friendly and its operation is quite simple.

We have found that RSA solves the problem of key agreement and key exchange generated in private-key cryptography algorithms but still there is lack of confidentiality. AES is a private key based algorithm that suffers from key distribution and key  agreement problems. However, the problem is solved in RSA algorithm but encryption and decryption take more time in RSA. Therefore, both the algorithms have their own merits and demerits. Based on the computation time, AES is faster compared to RSA. AES took an average of 4 seconds to transmit 8-bit message to the receiver, whereas RSA took 6 seconds to transmit 8-bit message.

# Future Scope
Additional features can be incorporated into this system if required. Since this project is limited to 1 km range due to use of HC12 module, long distance communication can also be implemented if we use more sophisticated modules like LoRa which has  range more than 10 km. The length of the message to be transmitted can also be increased by modifying the micro-controller program. This project is restricted to text message transmission. We can further incorporate type of the message like image, file and so on. To ensure high security, Elliptic Curve Digital Signature Algorithm (ECDSA) can be  used as a substitute of RSA algorithm module.
