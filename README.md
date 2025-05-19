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

# Sepolia Fucet

These are the test token because we can;t efford the etherum coin , also for the learning purpose we use them , these faucet can be get from the Google Cloud.

![image alt](https://github.com/Gautam-io-dev/Blockchain_learnings/blob/ea6d9ca887d3dd93afcdaa3cb69e4ebd674cd3a1/google%20cloud.png)

Here in the above Image you can see the Wallet Address where we have to add the our metmask wallet address then click on the recive button and when you refresh your metamask account you can see the faucets.

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

![image alt](https://github.com/Gautam-io-dev/Blockchain_learnings/blob/dd50129bda84acdb2bab3758bd5e0059c63b8ff4/DEPLOY1.png)

After Deploying we can see the green tick which show our contract is deployed on the blockchain

![image alt](https://github.com/Gautam-io-dev/Blockchain_learnings/blob/08d92da5a64227baf8f18a5f9642f16bf82bd216/DEPLOY.png)

Running the code:-

![image alt](https://github.com/Gautam-io-dev/Blockchain_learnings/blob/617546cdd8558606ce769faba2856f5eed727624/RUNNING%20OF%20CODE.png)

# blockchain Practicals:

**Question 1:Create a voting system with multiple candidates. Each address can vote only once.**

![image alt](https://github.com/Gautam-io-dev/Blockchain_learnings/blob/4d5515c61f57a72314564892d9e6a4ba50fa21d0/Question%201.png)
![image alt](https://github.com/Gautam-io-dev/Blockchain_learnings/blob/edaeb889d67a75c746ce66136a92232fc716265e/tranc%201.png)

**Question 2:Write a contract that manages a list of student records (name, roll number). Allow adding and retrieving student data.**

![image alt](https://github.com/Gautam-io-dev/Blockchain_learnings/blob/5e0f5a9303c11d920c0e4faf82cb5e06da62f044/Question%202.png)
![image alt](https://github.com/Gautam-io-dev/Blockchain_learnings/blob/e5b060960c1b193c8d36f03a25caff4e7480efa9/transc%202.png)

**Question 3:Develop a contract that only allows the deployer (owner) to call a specific function (use modifiers).**

![image alt](https://github.com/Gautam-io-dev/Blockchain_learnings/blob/b5ef4c1ca41fb73f2010255b950f14c1f5b80f3e/question3.png)
![image alt](https://github.com/Gautam-io-dev/Blockchain_learnings/blob/b9638c6cf58ac3228e383b4cd089932b13a9a552/transc%203.png)

**Questin 4:Write a contract where people can donate Ether and the top 3 donors are tracked.**

![image alt](https://github.com/Gautam-io-dev/Blockchain_learnings/blob/6c1d431e5074a1762bcdeda3056c619dbf2111f4/question%204.png)
![image alt](https://github.com/Gautam-io-dev/Blockchain_learnings/blob/6ea6fc4ed44601cb53a725fc2e5f8c011f56b371/transc%204.png)

**Question 5:Implement a simple auction system where users can place bids, and the highest bidder wins.**

![image alt](https://github.com/Gautam-io-dev/Blockchain_learnings/blob/af171ae4f5286ed8e9c43a075a6f20fee1be2be5/question%205.png)
![image alt](https://github.com/Gautam-io-dev/Blockchain_learnings/blob/76a6f802b3394135991acf8e0c0caad83d053232/transc%205.png)

**Question 6:Create a contract that splits incoming Ether between 3 fixed addresses.**

![image alt](https://github.com/Gautam-io-dev/Blockchain_learnings/blob/0300afe60fd0d7a1b2ac28a47306b9e0218bdacc/question%206.png)
![image alt](https://github.com/Gautam-io-dev/Blockchain_learnings/blob/77ab0c2e50f131ecd4bf637fa091e36f21d4f490/transc%206.png)
