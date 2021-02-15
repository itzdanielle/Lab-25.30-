# Lab-25.30-
#include <iostream>
using namespace std;

/* _Strings_
Examine the code and run the program to see how it works. 
Add the following functionality to the program:
1. Also print out the user's word in lowercase letters.
2. Have the user input a second word and store it in a string variable.
3. Output whether the 2 inputted strings are the same length or not.
4. Output whether the 2 inputted strings are case insensitive equal or not (For example, "dog" would be case insentitive equals to "DOG").
*/

int main() {
  string word, wordCap, wordCap2;
  int i;
  cout << "Please enter a word and press enter.\n";
  cin >> word;
  
  wordCap.resize(word.length()); // make wordCap the same length as word
  for(int i = 0; i < word.length(); i++) {
    wordCap[i] = toupper(word[i]);
  }
 wordCap2.resize(word.length()); // make wordCap the same length as word
  for(int i = 0; i < word.length(); i++) {
    wordCap2[i] = tolower(word[i]);
  }
  if (wordCap[i] == wordCap2[i] ) {
    cout << "Case insensitive equal" << endl;
    
  }
  if (wordCap[i] != wordCap2[i] ) {
    cout << "Not case insensitive equal" << endl;
  }
  if (word.length() == word.length()) {
    cout << "Are the same length" << endl;
  }
  if (word.length() != word.length()) {
    cout << "Are not the same length" << endl;
  }
  cout << "Your word capitalized: " << wordCap << endl;
  cout << "Your word has " << word.length() << " letters.\n";
  cout << "Your word not capitalized: " << wordCap2 << endl;
  cout << "Your word has " << word.length() << " letters.\n";
}





