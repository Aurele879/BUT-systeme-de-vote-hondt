# Hondt vote system

### /❗\ ONLY WORKS WITH C++ 17 AND OLDER VERSIONS /❗\

## ❔ How is this vote system working ?
We take the scores (number of votes) for each candidate/party, and we successively divide them by 1,2,3,4,… up to the number of seats to be filled (n), or n+1 times, to generate a set of quotients greater than the number of seats.

Once this is done, we rank all our division results (quotients) in descending order, taking care to retain the information of the candidate/party they refer to.

We allocate the n seats desired by taking the n highest quotients from our ordered list. The candidate/party to whom each of these top quotients refers is awarded one seat. For example: Party 'Banane' receives 3 seats because it appears 3 times in the list of the highest quotients.

## 🧠 Usage
First, you need to download the repository, compile the .c++ file, I recommend g++ because it is the only compiler I tested.
Then you need to open a terminal, and execute the program with this type of command : ./executable_of_the_program < entryx.txt

## 📖Entry files structure
You need to respect some things while doing your text files used for entry, you can reproduce the ones in the repository, keep in mind that you need to use the 4 first lines for the name of your candidates (you can only use the program with four candidates, one per line)
