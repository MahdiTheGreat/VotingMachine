# VotingMachine
an implementation of a voting machine,with a master arduino board sending the questions,and collecting the votes of the slave arduinos.

with a combined use of spi,i2c and uart transmition protocals,we are able to send all the questions to the voting machines at once,and then collect the results,with a round-robin
sort of way,while also enabling the voters to take back their votes,in case of a mistake.to send a vote,voter have to select the option they want,and then press +,and to take back a vote,voters have to select the option they have voted on,and then press the - button to take the vote back.

all the slaves have no internal memory,so the voting process is discrete.
