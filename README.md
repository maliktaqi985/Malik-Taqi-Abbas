Binary Search Implementation 
 
#include <iostream> #include <vector> using namespace std; 
 
int binarySearch(vector<int> arr, int target) {     int left = 0, right = arr.size() - 1;    
while (left <= right) {         int mid = left + (right - left) / 2;        
 if (arr[mid] == target)             return mid; // Target found         else if (arr[mid] < target)             left = mid + 1;         else             right = mid - 1; 
    }     return -1; // Target not found 
} 
 
int main() {     vector<int> arr = {2, 3, 4, 10, 40};     int target = 10; 
 
    int result = binarySearch(arr, target);     if (result != -1)         cout << "Binary Search: Target found at index " << result << endl; 
    else 
        cout << "Binary Search: Target not found." << endl; 
 
    return 0; 
} 
 
 
 
Linear Search Implementation 
 
 
#include <iostream> #include <vector> using namespace std; 
 
int linearSearch(vector<int> arr, int target) {     for (int i = 0; i < arr.size(); i++) {         if (arr[i] == target)             return i; // Target found 
    }     return -1; // Target not found 
} 
 
int main() {     vector<int> arr = {2, 3, 4, 10, 40};     int target = 10; 
 
    int result = linearSearch(arr, target);     if (result != -1) 
        cout << "Linear Search: Target found at index " << result << endl; 
    else         cout << "Linear Search: Target not found." << endl; 
 
    return 0; 
} 
How to Run the Program in Dev-C++ 
 
Open Dev-C++: Launch the Dev-C++ IDE on your system..
 
Create Separate Files: 
Create a new file for Binary Search (binary_search.cpp): 
Go to File > New > Source File. 
Paste the Binary Search code into the editor. 
Save the file as binary_search.cpp. 
Repeat the same steps for Linear Search (linear_search.cpp). 
 
Compile the Program: 
Open the desired file (e.g., binary_search.cpp) in Dev-C++. 
Click on Execute > Compile and Run or press F11. 
This will compile the code and execute it directly within the IDE. 
 
View Output: 
After running, the output will appear in the console window at the bottom of Dev-C++. 
 
Repeat for Other Program: 
Close the current file and open linear_search.cpp in Dev-C++. 
Compile and run it to view the Linear Search program output. 
 
 
 
 
Purpose of the Code
 
This project implements two fundamental searching algorithms: 
Binary Search: Efficiently finds the position of a target element in a sorted list. 
Linear Search: Iterates through the list to find the target element. 
 
 
 





Time Complexity 
 
Binary Search: 
 
Best Case:  O(1) 
Worst Case: O(logn) 
 
 
Linear Search: 
 
Best Case: O(1) 
Worst Case: O(n) 
 
 
_The End_
 
