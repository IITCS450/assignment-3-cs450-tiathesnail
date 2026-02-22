setup:
children inherent their parent's ticket amount on creation

Every time scheduler is run, the total amount of tickets of all runnable processes is calculated.
Then a random ticket is chosen withing that range, then cpu finds which process has that winning ticket.
Winning process is chosen to run, then scheduler finishes after that process returns.


Processes with higher ticket counts do seem to get chosen more often, but I had a hard time writing a program to test that. I think that xv6's printf or any other syscalls interfere with the scheduler in ways I do not know about.
