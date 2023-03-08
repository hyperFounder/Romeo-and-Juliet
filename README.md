# Client Server Application Romeo and Juliet

*Felipe Orihuela-Espina*

## About the assignment

- Deadline: Monday 6th-Mar-2023 at 16:00 (UK time).
- Late submissions policy: No late submissions allowed.
- What to submit: A single .zip file as explained in Section 4 Learning outcome: Design and implement server-side application software.

## Problem statement

In this exercise you are going to program a a well-known ordinary differential equation (ODE) known as Romeo and Juliet over a TCP/IP client-server architecture. Don’t worry, you do NOT need to know calculus at all or understand ODEs to solve the exercise; the method implementing the ODE will be provided to you, so you focus only on the TCP/IP client-server architecture.

The figurative scenario is a variant of the famous Romeo and Juliet play by William Shakespeare. Again, you do not have to have read the play in order to understand or solve the assignment. In the original tragedy, the two lovers face an impossible relation because of the ongoing rivalry between their families. Here, our scenario is just slightly different; whereby the playwriter, William Shakespeare, gets acquaintance with the two lovers and an exchange of love letters commence with the playwriter playing a kind of matchmaker between the two while writing the play about the love story. In this figurative scenario, the verses of the play correspond to the different values of the ODE over time.

In a more real scenario; you will be building a 1 client (the Playwriter) and 2 single-threaded servers (Romeo and Juliet) concurrent system. You are provided with templates for these three files with only a few gaps to be filled; the gaps control the client-server communication processes. The servers (Romeo and Juliet) are analgous in the service they provide although each one solve one of the equations of the Romeo and Juliet ODE. They are single-threaded. The client, i.e. the Playwriter, will be responsible to com- municate with the servers to get the ODE values over time (i.e. iterations). For each verse of the play (i.e. iteration of the ODE), the Playwriter will request the service from both servers and annotate their answers in the novel. At the end of the iterations, the novel will be dumped into a .csv file. The method to do so is also provided to you, so you do not have to worry about it.

In *all* classes, you are requested to treat exceptions in the method that first can raise them i.e. do not rely in throws clauses to deal with exceptions at a later stage. If some exceptions requires you to stop the execution of either the servers, or the client without a correct resolution of the request, make sure that in those cases you exit the program with code 1. Exit with code 0 if program execution is correct.

