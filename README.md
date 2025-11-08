#include <iostream>
using namespace std;

int main() {
    string word;
    int count = 0;

    cout << "Enter a 5-character word: ";
    cin >> word;

    // Check if input is exactly 5 characters long
    if (word.length() != 5) {
        cout << "Error: Please enter exactly 5 characters." << endl;
        return 1; // Exit with error code
    }

    // Count the number of 'a' or 'A'
    for (int i = 0; i < 5; i++) {
        if (word[i] == 'a' || word[i] == 'A') {
            count++;
        }
    }

    cout << "Number of 'a's in the word: " << count << endl;

    return 0;
}
