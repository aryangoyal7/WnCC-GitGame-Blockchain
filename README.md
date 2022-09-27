# GitGame - Hello Foss

You are a bunch unethical programmers, you built a program and fooled the world into thinking it’s a new kind of blockchain technology and it will  revolutionize financial systems of the world.
So people obviously jump on the wagon as it’s the new fad,  Elon also tweets about your blockchain technology and your tokens, people put their life saving in your virtual blockhain based bank as an investment in hope of the pipe dream that their deposits will surge.
</br>

Now, the catch in your blockchain program is that it’s not actually immutualable which is a fundamental property of this particular technology, you as an administrator have special access to re-write the ledger, hence you are going to perform a fraud.
You are planning to change the ledger logs (which are in form of commit messages) and steal money from people who put deposits in your virtual banking system.

Alrights, let's start:

Start with exploring the files provided to you , they have all the logs(in form of logx.txt files) which keep a track of all the transaction and there's a file of .txt type called Ledger which is supposed to be immutuable and keep a track as well and is open to everyone on the blockchain to see.
</br>

Read all the commit messages and log files to follow the sequence of transactions that have taken place, to commit fraud we'll create the following irregularities.

Task 1: create a new branch out of the master branch and name it "Danny_Ocean",  by creating this branch you have been empowered with ability to edit the so called 
immutable ledger, you have to edit the following statments in the newly created branch called "Danny_Ocean":

- >  "Bjarne Stroustrup deposists 5 eth , Total funds = 155eth should be changed" to </br>
 "Bjarne Stroustrup deposists 2 eth , Total funds = 152eth"
 
- >  "Vitalik Buterin withdraws  20 eth, total funds = 132eth"
to </br>
"Vitalik Buterin withdraws  50 eth, total funds = 102eth"

Commit the above made changes with a message "Job done by Danny".


Task 2: Now comeback to the master branch, there you have make some changes to the ledger as well, which is perfectly legal it's assumed that whatever happens in the master brancg allign with the ground truth.

Make the following chanage in the ledger:
- >  "Bjarne Stroustrup deposists 5 eth , Total funds = 155eth should be changed" to </br>
 "Bjarne Stroustrup deposists 5 eth."
 
- >  "Vitalik Buterin withdraws  20 eth, total funds = 132eth"
to </br>
"Vitalik Buterin withdraws  20 eth"

Commit the above made changes with a message "Job done, Ledger Updated".


Now merge these 2 branches with the changes you made.

What do you see? A merge conflict ? good! Your job is half done, now fix it via making the changes made in "Danny ocean" branch in the master branch as well.


Task 3: 

Open the git log and read all the commit messaged, you'll see they dont align with master branch now, hence we'll changes those as well now.

So, changes those messages to the new values specified in the previous tasks!
</br>

Hint: Use interactive git rebase

