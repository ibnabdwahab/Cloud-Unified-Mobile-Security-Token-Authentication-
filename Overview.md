******************************************************

    Secured OTP Authentication on Mobile Phone
    
******************************************************

The number of different identities and credentials used for authentication towards services on the Internet has increased beyond the manageable. Still, the most common authentication scheme is based on usernames and passwords. This is a weak authentication mechanism, which can be broken by eavesdropping on the network connection or by sloppy handling by the users (e.g. re-use of the same password for different services, writing down the passwords on paper etc.). Also, management of user credentials is a costly task for most companies, estimated by IDC to around 200-300USD pr. user/year. 

Several more secure solutions for electronic authentication exist, such as One-Time-Password (OTP) or Smart Card PKI solutions. They solve the security problem with passwords, but they most often increase the burden for the user. Extra hardware and software is required both for the user and service provider and they are often specific for each service so the user needs to deal with many different devices and procedures. Hence, better solutions for simplified, yet secure authentication, is required in the future.

The diagram above describes an authentication scheme based on a One-Time Password (OTP) MIDlet running on a mobile phone for unified authentication towards any type of service on the Internet. This authentication scheme would use the mobile phone as an authentication token. The GSM system is already well understood by the user and the proposed solution does not require any extra hardware device at the user side. The mobile phone has several advantages which can be exploited in user authentication:

• most people already have one

• the mobile phone has computing and communication capabilities that allows automation of the authentication process, relieving the user of this burden

• there are already good security mechanisms built into the GSM system that may be exploited

A system can authenticate a user to determine if the user is authorized to perform an electronic transaction or get access to information or a system. The authentication process begins with a client requesting a service which requires authentication. The client is asked to present a token to prove his identity. A token binds a user’s identity together with a secret and is given to the user during registration. When a user presents his token during authentication the authenticating party can verify the user’s identity since the token is unique for each user. 

When designing an authentication scheme which uses two separate devices which communicate over two different networks it is very important to ensure that it is the same user that controls both devices. This is done by ensuring that there is a “closed loop” going through all the components involved in the authentication as illustrated in the diagram. The loop starts in the device requesting the service, goes through the network with Service Provider (SP) and Authentication Server (AS) and then via the mobile phone and back to the initial device either by user interaction. 

The mobile OTP solution combines the simple and secure OTP principle with the iniquitousness of a GSM mobile phone. A Java MIDlet which can be installed on any Java enabled mobile phone transforms the phone into a secure OTP token which can be used to log in to any service on the Internet

The solution is based on a simple challenge-response protocol. When the user wants to log in he presents his username, and a challenge is sent to the user’s mobile phone. The OTP MIDlet installed on the phone generates an OTP from the challenge and sends it back to the server. The server verifies that the OTP is correct, and the user is authenticated as seen in the key exchange on the diagram

Conclusively, this secure authentication solution based on the OTP principle. It shows how an OTP MIDlet turns the mobile phone into a secure and user user friendly authentication token. The proposed solution eliminates weaknesses of existing similar solutions such as the need for time synchronization, possibility of man-in-the middle attacks and substantially improves the user-friendliness. It is therefore a very good alternative to the existing authentication solutions such as username-password and existing OTP solutions which require extra hardware and therefore put an extra burden on the user and increase the costs for the companies/service providers.
