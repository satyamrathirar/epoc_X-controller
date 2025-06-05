# epoc_X-controller
give keyboard and mouse inputs using EEG signals with the help of Emotiv Epoc X headset.\
Goal : to play video games just using your brain.\
Insights :
1. using Cortex API (provided by the emotiv) to make a communication channel between the headset and your code.
2. Working : data (command) coming from the headset, will be stored in the shared memory buffer (check send_command() in python/live_advance.py) from there, in the game, it will be checked which command is pushed into the buffer.\
earlier approach was to write the command into a text file and read it from there due to which a delay was seen there in the input because read/write operations are significatly slower than the shared memory buffer.