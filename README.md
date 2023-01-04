# palindrome
string = input("enter your string: ")
def is_palindrome(string):
    stripped_string = ''.join(a for a in string if a.isalnum()).lower()
    reverse_string = stripped_string[::-1]
    return stripped_string == reverse_string
if is_palindrome(string):
    print(f"{string} is palindrome")
else:
    print(f"{string} is not a palindrome")
