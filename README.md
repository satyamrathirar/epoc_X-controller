# epoc_X-controller
give keyboard and mouse inputs using EEG signals with the help of Emotiv Epoc X headset.\
Goal : to play video games just using your brain.\
Insights :
1. using Cortex API (provided by the emotiv) to make a communication channel between the headset and your code.
2. Working : data (command) coming from the headset, will be stored in the shared memory (check send_command() in python/live_advance.py) from there, in the game, it will be checked which command is pushed into the buffer.
