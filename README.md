# Lesson-14

    #include <iostream>
    #include <array>
    using namespace std;
    int main()
    {
        array <string, 4> arr = {"Mars Bar", "Snickers", "Bounty", "Wispa"};
        cout << arr.at(1) << endl;
        cout << arr[1] << endl;
        cout << arr.front() << endl;
        cout << arr.back() << endl;
        for (int i = 0;i < arr.size();i++) {
            cout << arr.at(i) << ", ";
        }
        cout << endl;
    }

sort

    #include <iostream>
    #include <array>
    #include <algorithm>
    using namespace std;
    int main()
    {
        array <int, 5> numbers = {33,5,7,99,83};
        sort(numbers.begin(), numbers.end());
        for(int num: numbers){
            cout << num << " ";
        }
    }
   
reverse

    #include <iostream>
    #include <array>
    #include <algorithm>
    using namespace std;
    int main()
    {
        array <int, 5> numbers = {33,5,7,99,83};
        reverse(numbers.begin(), numbers.end());
        for(int num: numbers){
            cout << num << " ";
        }
    }
