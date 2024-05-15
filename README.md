# Write program to display your name and perform following operations on it: 
Display n characters from left. (Accept n as input from the user)
Count the number of vowels. 
Reverse it. 
The code and its output must be explained technically. The explanation can be provided before or after the code, or in the form of comments within the code.

# Function to display n characters from the left of the string
def display_n_characters(name, n):
    print("Displaying", n, "characters from the left:", name[:n])

# Function to count the number of vowels in the string
def count_vowels(name):
    vowels = 'aeiouAEIOU'
    vowel_count = 0
    for char in name:
        if char in vowels:
            vowel_count += 1
    print("Number of vowels in the name:", vowel_count)

# Function to reverse the string
def reverse_string(name):
    print("Reversed name:", name[::-1])

# Main function
def main():
    name = input("Enter your name: ")
    n = int(input("Enter the number of characters you want to display from the left: "))
    
    # Display n characters from the left
    display_n_characters(name, n)
    
    # Count the number of vowels
    count_vowels(name)
    
    # Reverse the string
    reverse_string(name)

# Call the main function
if __name__ == "__main__":
    main()
