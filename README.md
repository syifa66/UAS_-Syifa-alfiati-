# include <iostream>
using namespace std;

int binarySearch(int arr[], int left, int right, int key) {
    while (left <= right) {
        int mid = left + (right - left) / 2;
        if (arr[mid] == key) {
            return mid;
        } else if (arr[mid] < key) {
            left = mid + 1;
        } else {
            right = mid - 1;
        }
    }
    return -1;
}

int main() {
	cout << "Nama : Syifa alfiati" << endl;
	cout << "Nim : 241011400831" << endl;
    int arr[] = {2, 3, 4, 10, 40};
    int size = sizeof(arr) / sizeof(arr[0]);
    int key = 10;
    int result = binarySearch(arr, 0, size - 1, key);
    (result == -1) ? cout << "Element not found" : cout << "Element found at index " << result;
    return 0;
}
