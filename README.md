# is_english.py

This Python script helps to identify if a given message is in English. It is roughly based on the percentage of words that are valid English words and the percentage of characters that are valid English characters.

## How it works

1. `load_dictionary()`: Loads a dictionary of English words from a file named 'dictionary.txt'.
2. `remove_non_letters(message)`: Removes all the characters from the message that are not letters or spaces.
3. `get_english_count(message)`: Calculates the percentage of words in the message that exist in the English language.
4. `is_english(message, word_percentage=20, letter_percentage=85)`: Returns True if the message is English, and False otherwise. By default, 20% of the words must exist in the dictionary file, and 85% of all the characters in the message must be letters or spaces (not punctuation or numbers).

## Usage

Here's an example of how to use this script:

```python
message = "Hello, how are you?"
if is_english(message):
    print("This message is in English.")
else:
    print("This message is not in English.")

```

Please note you need a dictionary file named 'dictionary.txt' in the same directory as the script for it to work.
