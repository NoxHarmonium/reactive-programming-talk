### Turning Push into Pull

- You can chain lots of functions together in expressive ways
- Transform functions can be sync or async

```javascript
fileAResult = readURL('http://example.org/fileA.txt')
fileBResult = readURL('http://example.org/fileB.txt')

combinedTextResult = when(fileAResult, fileBResult)
	.then(concat)	
	.then(capitalize)
	.then(trim)
	.then(print)
	.error(handleError)

```