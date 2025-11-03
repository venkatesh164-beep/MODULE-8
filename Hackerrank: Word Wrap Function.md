# 🔄 Hackerrank : # 📦 Python Word Wrap Function

This Python program defines a function that **wraps a long string into multiple lines**, ensuring each line does not exceed a specified width.

---

## 🎯 Aim

To write a Python function that takes a long string and a specified width, and returns the string formatted with line breaks such that each line has **at most the given width**.

---

## 🧠 Algorithm

1. **Start** the program.
2. Define a function `wrap(string, max_width)`:
   - Create an empty list `wrapped_lines` to store parts of the string.
   - Loop through the string using steps of `max_width`.
   - In each iteration, extract a substring of length `max_width`.
   - Append this substring to the list.
3. Join the list with `\n` to create the final string.
4. Return the result.
5. **End** the program.

---


## 🧪 Program
def wrap(string, max_width):<br>
    wrapped_lines = []<br>
    for i in range(0, len(string), max_width):<br>
        wrapped_lines.append(string[i:i+max_width])<br>
    return '\n'.join(wrapped_lines)<br>

text = input("Enter a long string: ")<br>
width = int(input("Enter max width: "))<br>
print("\nWrapped Text:\n")<br>
print(wrap(text, width))

## Sample Output
<img width="738" height="400" alt="image" src="https://github.com/user-attachments/assets/af0e95a2-459c-468a-8520-ddd15152fde7" />

## Result
Program is verified successfully.
