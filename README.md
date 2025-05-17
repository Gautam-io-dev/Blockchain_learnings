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

![image alt]()

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

    
