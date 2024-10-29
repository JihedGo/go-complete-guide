Array: fixed length list of things

Slice: an array that can grow or shrink

* whenever  array or slice, every single record inside of it must be of an identical type.

Go is not an object oriented programming language, so there's no idea classes inside of Go.


```go
type deck []string
func (d deck) print() {  
	for i, card := ranged 
            {  
		fmt.Println(i, card)  
	    }
}
```

d is a reference to cards array

if we were working with any other type of language specifically , like if we were working with Python , Ruby , js 

you could think this d receiver variable as being very similar to the word this or the word self.

with go we very specifically by convention we never use the word this or self.

you might be curious about is why we called d in the actual implementation.

by convention we usually refer to the receiver with a one or two letter abbreviation that matches the type that we of the receiver.

in that case, because our receiver is of type deck , we refer to the actual copy where the reference to the actual deck simply as d.

```go
for i, suit:=rangecardSuits {  
	for j, value:=range cardValues {  
		cards = append(cards, value+" of "+suit)  
	}  
}
```

you'll notice i and j here they were the index of every suit in value in both those slices. but we never have to actually use these indices at any point for putting this slice of cards together.

* whenever you have some variable that you don't actually have to use , we always replace it with underscore which tells go, hey , we understand that there is a variable here , we just don't care about it and we don't want to use it.
