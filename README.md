## VoIP using SIP Protocol

SIP (Session Initiation Protocol), one of the protocols used in VoIP, based on HTTP, responsible for starting, establishing, changing and ending sessions. SIP works on a client/server architecture, it is the signaling protocol and dictates the rules and how end-to-end communication will occur. It uses other protocols and resources such as RTCP (Real-Time Control Protocol), which will control the RTP (Real-Time Transport Protocol), responsible for “voice transport” using UDP (User Datagram Protocol); TCP (Transmission Control Protocol), which is used at the beginning to configure the call and HTTP (HyperText Transfer Protocol), used for Response Codes when accepting the connection.

It is worth remembering that VoIP, or Voice over Internet Protocol, is a technology that allows you to make voice calls using an internet connection instead of a traditional telephone line.

For this example of the SIP protocol, we will use Asterisk and FreePBX. Asterisk is an open-source software that functions as a Private Branch Exchange (PBX), 
while FreePBX is a graphical interface for managing Asterisk. Don't worry, this will be explained in more detail later on.





