### Turning Push into Pull

- Reactive programming makes asynchronous events into a form of pull programming
- Code is now in order of execution
- Easy to read
- concat() and print() functions reusable

```javascript
fileAResult = readURL('http://example.org/fileA.txt')
fileBResult = readURL('http://example.org/fileB.txt')

when(fileAResult, fileBResult)
	.then(concat)
	.then(print)

```

