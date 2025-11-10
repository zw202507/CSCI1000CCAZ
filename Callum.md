#H1 this is Callum's folder to edit 
> this is quote block
> it can spam a few lines 

#include <iostream>
#include <string>
using namespace std;

int countCharacter(string array[], int size, char ch)
{
    int count = 0;

    for (int i = 0; i < size; ++i)
    {
        for (int j = 0; j < array[i].length(); ++j)
        {
            if (array[i][j] == ch)
            {
                ++count;
            }
        }
    }

    return count;
}

// Example usage
int main()
{
    string array[] = {"elephant", "english", "elegant", "america", "united", "apple"};
    int size = sizeof(array) / sizeof(array[0]);
    char ch = 'e';

    int result = countCharacter(array, size, ch);
    cout << "The character '" << ch << "' appears " << result << " times." << endl;

    return 0;
}

