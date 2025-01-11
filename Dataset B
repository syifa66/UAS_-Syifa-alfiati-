#include <iostream>
using namespace std;

int linearSearch(int arr[], int size, int key) {
    for (int i = 0; i < size; i++) {
        if (arr[i] == key) {
            return i;
        }
    }
    return -1;
}

int main() {
	cout << "Nama :Syifa alfiati" << endl;
	cout << "Nim : 241011400831" <<endl;
    int arr[] = {5, 3, 10, 1, 4};
    int size = sizeof(arr) / sizeof(arr[0]);
    int key = 10;
    int result = linearSearch(arr, size, key);
    (result == -1) ? cout << "Element not found" : cout << "Element found at index " << result;
    return 0;
}
