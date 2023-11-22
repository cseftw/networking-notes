# Understanding FTP

## What is FTP ?

**File Transfer Protocol (FTP) is, as the name suggests , a protocol used to allow remote transfer of files over a network. It uses a client-server model to do this, and- as we'll come on to later- relays commands and data in a very efficient way.**

## How does FTP work ?

**A typical FTP session operates using two channels:**

* **a command (sometimes called the control) channel**
* **a data channel.**

**As their names imply, the command channel is used for transmitting commands as well as replies to those commands, while the data channel is used for transferring data.**

**FTP operates using a client-server protocol. The client initiates a connection with the server, the server validates whatever login credentials are provided and then opens the session**

**While the session is open, the client may execute FTP commands on the server.**

## Active vs Passive&#x20;

**The FTP server may support either Active or Passive connections, or both.**&#x20;

* **In an Active FTP connection, the client opens a port and listens. The server is required to actively connect to it.**&#x20;
* **In a Passive FTP connection, the server opens a port and listens (passively) and the client connects to it.**&#x20;

**What's the standard FTP port?**

```
21
```

**What communications model does FTP use?**

```
client-server
```

**How many modes of FTP connection are there?**

```
2 : Active & Passive
```

**Connecting with FTP :**&#x20;

```
ftp <ip> <port>
```
