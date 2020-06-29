How the application build the flag:

1) the application load libff which are a modified version of frida gadgets
2) the agent loads the ducktape compiled, obfuscated script in libcrypto.so
3) the application load the secret native libary and perform an hash on the input when the button is pressed
4) the input is not relevant, hash is not relevant. 
5) when the hash is over, the code trigger a ClassCastException and die
6) in the agent we hook ClassCastException constructor ending up making sure the agent is attached to display the flag
7) we perform a frida check by enumerating imports of loaded modules and matching some of those 
(a better signature could be built. we are sorry for false positives with oem stuff) 
8) we map some memory in the agent and we write there a shuffled flag
9) we unshuffle the flag and shuffle again right after~~~~