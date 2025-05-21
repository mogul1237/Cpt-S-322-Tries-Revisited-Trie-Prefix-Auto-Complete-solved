# Cpt-S-322-Tries-Revisited-Trie-Prefix-Auto-Complete-solved

Download Here: [Cpt S 322 Tries Revisited: Trie Prefix Auto-Complete solved](https://jarviscodinghub.com/assignment/tries-revisited-trie-prefix-auto-complete-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

Build a basic WinForms application that has one text box that allows the user to type in a word.
Have a list box below the text box in the interface that lists all words from the supplied dictionary that
start with the prefix that the user typed in. The image below shows what your interface might look like.
To achieve this, you will need to build a trie for the array of strings loaded from the dictionary.
An “academic word list” text file that was obtained from
https://oald8.oxfordlearnersdictionaries.com/academic/ is included in the .zip file for this assignment. Do
not alter this file in any way.
2 of 4
Build the trie initially by adding all words in dictionary. Remember that you’ll start back at the
root for each new word. If you write an “InsertString” or “AddString” method to add a string to the trie
then you can just call that in a loop to add each word to the trie.
After the trie is built, get the prefix string from the user and then display all strings that start
with this prefix. Trace down the trie to consume all characters in the prefix. If you can’t consume all
characters then there are no strings in your dictionary that start with that prefix. Otherwise you’ll end at
a node that is the parent for all strings that start with this prefix. Enumerate all leaf nodes under this
parent to find the strings that start with the prefix. Display each one.
As a simple example, suppose your dictionary has the words: “apply appreciate apprehension
application applicable”. The trie for these 5 words looks like this:
3 of 4
If the user types in “appr”, then your traversal is represented by the light blue nodes in the
image below. The green nodes represent the leaves below that correspond to the ending points of
words that start with “appr”. So in this case the output should be “appreciate” and “apprehension”.
