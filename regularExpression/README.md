# Regular Expression

Regular Expression for Banglagesh with country code, min==max==13 characters(start with 8801):
-
- Regular expression of Bangladeshi phone numbers(what i want) where **number of characters=13** , **start with 8801**, the **`5th` character can be `3 to 9` not `0, 1, 2`**, and the other **8 characters can be `0 to 9`**.==> `^8801[3-9]\d{8}$`

Regex quick reference :
-
```
[abc]	A single character of: a, b, or c
[^abc]	Any single character except: a, b, or c
[a-z]	Any single character in the range a-z
[a-zA-Z]	Any single character in the range a-z or A-Z
^	Start of line
$	End of line
\A	Start of string
\z	End of string
.	Any single character
\s	Any whitespace character
\S	Any non-whitespace character
\d	Any digit
\D	Any non-digit
\w	Any word character (letter, number, underscore)
\W	Any non-word character
\b	Any word boundary
(...)	Capture everything enclosed
(a|b)	a or b
a?	Zero or one of a
a*	Zero or more of a
a+	One or more of a
a{3}	Exactly 3 of a
a{3,}	3 or more of a
a{3,6}	Between 3 and 6 of a
```

Operators of Bangladesh:
-
- 13 and 17 - Grameenphone

- 14 and 19 - Banglalink

- 15 - TeleTalk

- 16 and 18 - Robi

- 10, 11, 12 - Not in use

![alt text](https://github.com/aa-nadim/how-to/blob/main/regularExpression/re.png?raw=true)

for test:
-
- `https://rubular.com/r/3tI2ute1lWRz7r`