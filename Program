def linear_search(arr, target):
    for i in range(len(arr)):
        if arr[i] == target:
            return i
    return -1


def binary_search(arr, target):
    low = 0
    high = len(arr) - 1

    while low <= high:
        mid = (low + high) // 2
        if arr[mid] == target:
            return mid
        elif arr[mid] < target:
            low = mid + 1
        else:
            high = mid - 1
    return -1


def main():
    print("Welcome to the Search Algorithms Program!")
    print("Please choose a search algorithm to test:")
    print("1. Linear Search")
    print("2. Binary Search")

    choice = int(input("Enter your choice (1 or 2): "))

    arr = list(map(int, input("Enter the list of numbers (space-separated): ").split()))
    target = int(input("Enter the target number to search for: "))

    if choice == 1:
        # Linear Search
        result = linear_search(arr, target)
        if result != -1:
            print(f"Linear Search: Target found at index {result}")
        else:
            print("Linear Search: Target not found in the list")
    elif choice == 2:
        # Binary Search
        arr.sort()  # Sorting the array for Binary Search
        print(f"Sorted list for Binary Search: {arr}")
        result = binary_search(arr, target)
        if result != -1:
            print(f"Binary Search: Target found at index {result}")
        else:
            print("Binary Search: Target not found in the list")
    else:
        print("Invalid choice! Please select 1 or 2.")


if __name__ == "__main__":
    main()
