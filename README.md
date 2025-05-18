# Blockchain_learnings

# BASIC COMMAND TO INSTALL GOLANG AND FABRIC

To update the system:-
                         
    sudo apt update

To install golang-go:-

    sudo apt install golang-go

To install docker:-

    sudo snap install docker

To install git:-

    sudo apt install git

To install fabric-samples:-

    git clone -b main https://github.com/hyperledger/fabric-samples.git

to install curl:-

    sudo apt install curl

To get in fabric-samples:-

    cd fabric-samples

To pull hyperledger docker image:-

    sudo bash
   
    curl -sSL https://bit.ly/2ysbOFE | bash -s

To get into test-network:-

    cd test-network

To up the network:-

    ./network.sh

    ./network.sh up

To create channel:-

    ./network.sh createChannel

To down the network:-

    ./network.sh down

![image alt](https://github.com/Gautam-io-dev/Blockchain_learnings/blob/a555212dfe5109d74f0418b65bedd473601d83a0/terminal_stuff.jpg)

To install IPFS:-

    wget https://dist.ipfs.tech/kubo/v0.32.1/kubo_v0.32.1_linux-amd64.tar.gz

To use kubo:-

    tar -xvzf kubo_v0.32.1_linux-amd64.tar.gz

To get into kubo directory:-

    cd kubo

To move to local bin:-

    sudo bash install.sh

To initialise IPFS:-

    ipfs init
    
To use daemon:-

    ipfs daemon

![image alt]()

To run ipfs daemon in background:-

    ipfs.log 2>&1 &

To add file:-

    echo "Hello, IPFS!" > hello.txt
    ipfs add hello.txt
    ipfs cat <CID>

![image alt]()

To add a directory:-

    mkdir myfolder
    echo "File 1 content" > myfolder/file1.txt
    echo "File 2 content" > myfolder/file2.txt
    ipfs add -r myfolder

![image alt]()

lists running processes:-

    ps aux | grep ipfs

To kill the process:-

    kill <PID>

Encrypting and Decrypting:-

    echo "Hello, bruh" > myfile.txt
    ipfs add myfile.txt
    openssl enc -aes-256-cbc -pbkdf2 -iter 100000 -salt -in myfile.txt -out myfile_encrypted.txt -pass pass:yourpassword
    ipfs add myfile_encrypted.txt
    cat myfile_encrypted.txt
    openssl enc -d -aes-256-cbc -pbkdf2 -iter 100000 -in myfile_encrypted.txt -out decrypted_file.txt -pass pass:yourpassword
    cat decrypted_file.txt
    ipfs add decrypted_file.txt

![image alt]()

To add audio :-

    ipfs add <audio-path>

![image alt]()

To add video:-

    ipfs add <video-path>

![image alt]()

    
# METAMASK

The metamask account is our wallet where it store the token , like sepolia faucet which are the test token , with the help of metamask wallet we will do the transaction and deploy our smart contract on the blockchain.

![image alt](https://github.com/Gautam-io-dev/Blockchain_learnings/blob/a3154de05ade31f63a71de967eadd061d02f5827/meta%20mask.png)


# Solidity:

We write our smart contract in the solidity language .

To use this Language I have used the Remix ide website where I can deploy my contract for free also we can use our metamask account to know how to make transcation through that.

![image alt](https://github.com/Gautam-io-dev/Blockchain_learnings/blob/693e8191b2c5ea70e6d31cbc0b698786601be5a2/remix%20ide%20front.png)

![image alt](https://github.com/Gautam-io-dev/Blockchain_learnings/blob/c2b63875ab895097cf0c913e84bd20064086df28/solidity.png)

In above Image , the file explore saves our contracts.

Here’s an intermediate-level Solidity smart contract for a crowdfunding platform, which introduces several important concepts:
	•	Structs
	•	Mappings
	•	Modifier-based access control
	•	Event logging
	•	Withdrawal pattern


CODE:-

![image alt](https://github.com/Gautam-io-dev/Blockchain_learnings/blob/30a4f1340d36c8615a8f12a0199978c8736018d3/code%20.png)

Compiling the code:-

![image alt](https://github.com/Gautam-io-dev/Blockchain_learnings/blob/426e5e0d9c34f135603f8eab51311a32e243a213/compile.png)
![image alt](https://github.com/Gautam-io-dev/Blockchain_learnings/blob/1acbabfdd81eab9385684434f1fe58db4ff69a15/compile2.png)

Deploying on blockchain:-

![image alt]()
After Deploying we can see the green tick which show our contract is deployed on the blockchain

![image alt]()

Running the code:-

![image alt]()
