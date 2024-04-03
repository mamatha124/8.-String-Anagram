# 8.-String-Anagram in python
s1 = input()
s2 = input()
len1 = len(s1)
len2 = len(s2)
found = 0
notFound = 0
if len1 == len2:
    for i in range(len1):
        found = 0
        for j in range(len2):
            if s1[i] == s2[j]:
                found = 1
                break
        if found == 0:
            notFound = 1
            break
    if notFound == 1:
        print("Not Anagram")
    else:
        print("Anagram")
else:
    print("Not Anagram")
