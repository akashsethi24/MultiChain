# MultiChain

How to Install and Create BlockChain with Multichain

# <h2>How to install Multichain </h2>
  -  <b>Linux</b> <br>
  Open Terminal and run the following commands<br>
  ```
       cd /tmp 
  ``` <br>
  ```
       wget http://www.multichain.com/download/multichain-1.0-alpha-25.tar.gz
  ``` <br>
  ```
       tar -xvzf multichain-1.0-alpha-25.tar.gz
  ``` <br>
  ```
       cd multichain-1.0-alpha-25
  ``` <br>
  ```
       sudo mv multichaind multichain-cli multichain-util /usr/local/bin
  ``` <br>
  -  <b>Windows</b> <br><br>
       Download [MultiChain](http://www.multichain.com/download/multichain-windows-1.0-alpha-25.zip) and extract its content to your chosen directory

# <h2>How to Create and Connect to a BlockChain</h2>
   Open Terminal and run the following commands <br>
         ``` -  multichain-util create [chain-name] ``` <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; This command will create a BlockChain with given name Now you can manage the various configurations in params.dat file. you can find params.dat file in  ```/home/user/.multichain/[chain-name] ``` directory.<br><br>
        ``` - multichaind [chain-name] -daemon ``` <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; This command will start the BlockChain node and will lock the content of params.dat file. A node address such as ```chain-name@ip-address:port``` will be the output. this node address allow other nodes to easily connect.

