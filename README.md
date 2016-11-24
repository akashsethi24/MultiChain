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
  -  <b>Windows</b> <br>
       Download [MultiChain](http://www.multichain.com/download/multichain-windows-1.0-alpha-25.zip) and extract its content to your chosen directory

# <h2>How to Create and Connect to a BlockChain</h2>
   Open Terminal and run the following commands <br>
         <b>``` -  multichain-util create [chain-name] ```</b> <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; This command will create a BlockChain with given name Now you can manage the various configurations in params.dat file. you can find params.dat file in  ```/home/user/.multichain/[chain-name] ``` directory.<br><br>
        <b>``` - multichaind [chain-name] -daemon ``` </b><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; This command will start the BlockChain node and will lock the content of params.dat file. A node address such as ```chain-name@ip-address:port``` will be the output. this node address allow other nodes to easily connect.<br><br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Now the BlockChain has been created and started. To connect to the blockchain, first obtain the node address from any node which is already connected. and run the following command <br>
         <b>``` - multichaind nodeAddess -deamon ```</b><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  This command will connect you to the BlockChain. nodeAddress will be something like this ``` chain-naim@pAddress:port``` <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  example ``` chain1@12.34.56.12:5050```
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  - If the BlockChain is Private then the output of the command will contain <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ```your address``` in form of some random Aplhanumeric values. Admin of the BlockChain need to grant permissions on <br><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ```your address``` . you can find [here](http://www.multichain.com/developers/json-rpc-api/) more about permission grant under Permission Managment Section.<br>
      - Once the permissions are granted then you can easily connect to BlockChain with ``` - multichaind nodeAddess -deamon ``` &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;command.<br><br>
      
#<h2> Using Command-line Interface</h2><br><br>
  <b>``` - multichain-cli [chain-name] ```</b><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; This command wil open the cli for BlockChain you are connected to. This CLI will only work if you are connected the &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;BlockChain.<br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Now you can try various commands like ``` getinfo``` for general informations about nodes, balance etc. ```getaddresses``` &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; for yoru address. you can send currency to someone else by ``` send [other_person_address] amount``` command. <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - You can find all command [here](http://www.multichain.com/developers/json-rpc-api/)
