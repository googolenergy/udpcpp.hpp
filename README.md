# udpcpp.hpp (v1.0)

<img src="./images/udpcpp_logo_public.png" alt="udpcpp_logo_public" width="150" style="margin-right: 15px;">
<p><b>"udpcpp.hpp"</b> is a C++ library especially made to implement UDP communication in your projects. It provides an easy-to-use interface for sending and receiving UDP packets with minimal setup.

Currently the <b>initial version 1.0</b> supports sending & listening only to/form `127.0.0.1`. The following template is designed to work with only <a href="https://visualstudio.microsoft.com/vs/older-downloads/">Visual Studio 2019</a>. The purpose of <i>localhost-support-only</i> was designed to establish communicaiton between various applicaitons. Future versions of <b>udpcpp.hpp</b> will have power to communicate any hardware or software that supports UDP protocol.

Download <b>udpcpp.hpp (1.0)</b> <a href="https://drive.google.com/file/d/19bH2PnbeMV1ztyC8UBZ36HehlgtVG70C/view?usp=sharing">here</a>.

## API Docs

This library is minimal & compact to implement. There are mainly two methods, `udpSend()` and `udpReadNL()`
<br>
1.  `udpSend()` is used to send messages to the server. It takes two parameters, `int port` and `std::string message`. `port` is the nerwork port for which the message is sent to & `message` is a string of the actual message.

2.  `udpReadNL()` is used to read the incomming messages from the host. <b>NL</b> stands for "New Line", it reads one entire line when called. `udpReadNL()` takes only one parameter i.e., `int port` which is the port number from where it starts listening to the incomming traffic. This funciton returns a `std::string` value which can be used further.
