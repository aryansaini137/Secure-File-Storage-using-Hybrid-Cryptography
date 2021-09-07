# Secure-File-Storage-using-Hybrid-Cryptography

# Methodology
To achieve the above goal, the following methodology needs to be followed:
 1.Load the file on the server.
 2.Dividing the uploaded file into N parts.
 3.Encrypting all the parts of the file using any one of the selected algorithms (Algorithm is changed with every part in round robin fashion).
 4.The keys for cryptography algorithms is then secured using a different algorithm and the key for this algorithm is provided to the user as public key.

After the above 4 steps you will have a N files which are in encrypted form which are stored on the server and a key which is downloaded as public key for decrypting the file and downloading it.

To restore the file, follow the following steps:

Load the key on the server.
 1.Decrypt the keys of the algorithms.
 2.Decrypt all the N parts of the file using the same algorithms which were used to encrypt them.
 3.Combine all the N parts to form the original file and provide it to the user for downloading.
