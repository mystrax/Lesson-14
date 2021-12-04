# Lesson-14

random

    #include <iostream>
    #include <string>
    #include <algorithm>
    #include <exception>
    #include <array>
    #include <random>
    using namespace std;

    int main()
    {
        //include srand to make the random generated numbers different, 
    //if you want differenet output each time, each the seed or you can also use the % logic
        srand(7);
        array<int,10> randomArry;
        for (int i = 0; i < 10; i++)
        {
            randomArry[i] = rand();
            cout << randomArry[i] << endl;
            }

    }
  
  ---
  

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

1000 numbers within 1-100

    #include <iostream>
    #include <array>
    #include <algorithm>
    using namespace std;
    int main()
    {
        int randomArry[1000];
        int j = 0;
        for (int i = 0;i < 1000;i++)
        {
            randomArry[i] = rand() % 100;
            cout << randomArry[i] << endl;
            if (randomArry[i] == 6) {
                cout << randomArry[i] << endl;
                j++;
            }
            else 
            {
                continue;
            }
        }
        cout << " Number 6 showed up: " << j << endl;
    }

largest

    #include <iostream>
    #include <array>
    using namespace std;
    int main() 
    {
        int User[10];
        int i;
        int max = User[0];
        for (i = 0; i < 10; i++)
       {
            cin >> User[i];
            if (User[i] > max) 
            {
                max = User[i];
            }
        }
        cout << "Largest Number inserted: " << max;
        return 0;
    }
    
Smallest

    #include <iostream>
    #include <array>
    using namespace std;
    int main()
    {

        int User[10];
        int i;
        int max;
        for (i = 0; i < 10; i++) 
        {
            cin >> User[i];
            max = User[0];
        }
        for (i = 0; i < 10; i++)
        {
            if (User[i] < max) 
            {
                max = User[i];
            }
        }
        cout << "smallest Number inserted: " << max;
        return 0;
    }
