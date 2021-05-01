# QuantCertificate

 A website that uses the notion of qubits in quantum key exchange over the quantum channel to secure candidate certicates provided by a specic institution. It effectively utilizes the quantum digital signature technique in which symmetric key cryptography is used. Random basis for each bit of the message will be selected on the sender's side, which is private to the sender and will be encoded using basis and sent then each qubit will be randomly calculated at the receiver's end, which will be private to the receiver. Now, both sender and receiver will publicly share basis that they used for every qubit if receiver measured the qubit in a similar basis which sender prepared it in, then it will be uses to form part of their shared secret key, otherwise message shared will be discard for that particular bit.Lastly, secret key is used for both sender and the receiver in order to encrypt and decry-pt information which will be hashed in form of image of 256 bits using wavelet transformation at the sender's end and AES(Advanced encryption standards) is implemented on hashed message and the secret key for encryption of the information and then that encrypted message is stored in the database and to view message at receiver’s again AES is applied on the message received.

Setup:
```
git clone https://github.com/Kinshukg04/Crypto_project.git
cd flask-login
virtualenv flask -p python3
source flask/bin/activate
pip3 install -r requirements.txt
python3 app.py
```

Then open ```http://localhost:5000/``` in a web-browser.
