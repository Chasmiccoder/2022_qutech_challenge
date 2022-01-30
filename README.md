<p align="center">
  <img width="300" height="300" src="https://user-images.githubusercontent.com/68393451/151703663-3cf07b92-5ccb-4ab3-9335-e103a2943bc1.svg">
</p>


# Q-Sup
A web-based interface to perform QKD.

# Abstract

Here we propose an innovative way of secure key distribution using a web interface. Two users login to a server where they input a randomly generated number sequence with three digits. Depending on the input string, measurements are performed on an entangled state (Here, we use the anti-correlated bell state). For an N bit input, N bell-states are required. Then the users communicate their measurement labelings through a classical channel. They keep those particular measurement bits, for which the index of the input string is equal, and discard the remaining bits. Now the two users have inverted bit strings. One of the users flips their bit (also decided through the classical communication channel to get the secured key. This idea can be extended by using an n-qubit entangled state for n users. Our protocol is based on the E91 protocol.



# Walkthrough

1. User A logs in to the server.
2. The user then inputs a randomly generated string of three digits.
3. Based on the input string, the server performs partial measurements on a sequence of entangled states and returns the result to the user.
4. User B logs in to the server and does the same.
5. The two users discuss their measurement sequence on a classical channel.
6. They retain the bits on those indices for which their measurements were performed on the same index.
7. One of the users inverts their bit string.

# Theory

Our key distribution technique is based on the E91 protocol. Depending on the initial state, some users may have to invert their strings to get the key.

To learn more about the protocol go to this link: https://en.wikipedia.org/wiki/Quantum_key_distribution#E91_protocol:_Artur_Ekert_.281991.29

![image](https://user-images.githubusercontent.com/68393451/151702199-7d0bac60-b2e0-405f-a7d0-5ac462314bba.png)

Image source: [link](https://medium.com/@qcgiitr/fundamentals-of-quantum-key-distribution-bb84-b92-e91-protocols-e1373b683ead)







Set up -

```
pip install -r requirements.txt
python -m flask run
```

Check out the [Quantum Key Distribution - Ekert 91 Protocol notebook](https://github.com/Chasmiccoder/Q-Sup/blob/master/Quantum%20Key%20Distribution%20-%20Ekert%2091%20Protocol.ipynb) to understand how we deployed the QKD E91 protocol to make Q-Sup work.

Resources -
1. <a href="https://www.freepik.com/vectors/background">Background vector created by coolvector - www.freepik.com</a>
2. [Qiskit - Quantum Key Distribution](https://qiskit.org/textbook/ch-algorithms/quantum-key-distribution.html)
3. [Fundamentals of Quantum Key Distribution](https://medium.com/@qcgiitr/fundamentals-of-quantum-key-distribution-bb84-b92-e91-protocols-e1373b683ead)
4. [QKDs and secret keys](https://mpl.mpg.de/fileadmin/user_upload/Chekhova_Research_Group/Lecture_4_12.pdf)

# Experience

Our team would like to thank the entire organizing team of iQuHACK for giving us this splendid opportunity to learn. We are thankful and grateful to have been involved in this enticing quantum quest !


Enjoy the Quantum Cruise !
Regards, 
Team Q-Sup
Angela, Aryaman, Galeinston, Rita and Sahil
