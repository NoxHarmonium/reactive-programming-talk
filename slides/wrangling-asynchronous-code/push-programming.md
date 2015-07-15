### Push Programming

```javascript
filesRead = 0; textA = null; textB = null

function receivedData() {
	if (filesRead++ == 2) {
		combinedText = concat(textA, textB)
		print(combinedText)
	}
}

readURL('http://example.org/fileA.txt', function(recvTextA) {
	textA = recvTextA
	receivedData()
})
readURL('http://example.org/fileB.txt', function(recvTextB) {
	textB = recvTextB
	receivedData()
})
```
