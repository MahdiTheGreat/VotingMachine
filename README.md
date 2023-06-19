# VotingMachine
an implementation of a voting machine,with a master arduino board sending the questions,and collecting the votes of the slave arduinos.

with a combined use of spi,i2c and uart transmition protocals,we are able to send all the questions to the voting machines at once,and then collect the results,with round-robin scheduling, while also enabling the voters to take back their votes, in case of a mistake.

to send a vote, voter has to select the option they want and then press +. to take back a vote, voters have to select the option they have voted on,and then press the - button to take the vote back.

all the slaves have no internal memory, so the voting process is discrete.

the implementation is done with the help of the arduino ide and the proteus envirement.

the implementation supports three scenarios:
1-we only use uart
2-three slave use uart and the fourth one uses i2c
3-like 3,but now 2 slaves use i2c,and we can expand this for 2^7-1 slaves
