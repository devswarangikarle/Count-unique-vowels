# Count-unique-vowels
Count the number of unique vowels in a given string 's'. Input The First line of input contains string 's'.  Constraints:- 1 ≤ s.length ≤ 105 The variable 's' consists exclusively of lowercase English letters. Output Print the number of unique vowels in a given string 's'.

def count_unique_vowels(s):
    vowels = set("aeiou")
    unique_vowels = set()
    for char in s:
        if char in vowels:
            unique_vowels.add(char)
    return len(unique_vowels)

s = input().strip()

print(count_unique_vowels(s))
