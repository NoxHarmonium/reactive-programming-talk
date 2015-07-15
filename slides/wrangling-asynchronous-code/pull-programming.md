### Pull Programming

- Data was 'pulled' from other sources synchronously.
- You had a guarantee that the execution will not proceed until each line is finished.

```javascript
textA = readFile('fileA.txt')
textB = readFile('fileB.txt')

combinedText = concat(textA, textB)

print(combinedText)

```

- Easy to follow, most programming languages we use were designed on this model