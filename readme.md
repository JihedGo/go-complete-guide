# Go Packages

```go
package main

import "fmt"

func main() {
	fmt.Println("Hi there !")
}

```

package = project = workspace

it is a collection of common source code files.

the only requirement for every file inside of a package is that the first line of each file **must declare the package that it belongs to.**

why we called our package main ?

inside of go , there are two different types of packages 

* Executable:
  is one that when compiled splits out an actual run able file an executable file.
  is usually used for actually doing something.
* Reusable:
  you can think of these as being like code dependencies.
  these are packages that are not used to say like double click on and execute, instead , we put in a lot of reusable logic or helper functions that will just help us reuse some code.

how do we know if we are making an executable package or a resusable one?

actually the name of the package that you use that determine whether you are making an executable or dependency type package.specifically , the word main is used to make an executable type package.

if we had used any other name than name for our package besides main , it would not split out an acutal executable file.

# Import statements

the import statement is used to give our package access to some code that is written inside of another package.

`import "fmt"`

means give my package main access to all the code and all functionality that is contained inside of the other package called fmt.

fmt is the name of standard library package that is included with go programming language by default.

fmt itself is a kind of a shortened form of the word format.

fmt library is used to print out a lot of different information specifically to the terminal, just to give you a better sense of debugging and stuff like that.

# File Organization

```go
func main(){}
```

func is a short of function.

it's always going to be the exact same pattern inside of every single file that we ever create :

at the very top we're always going to place our package declaration.

then right underneath that , we will list out all the other packages that we might need to import into this file.(fmt, io, etc.).

after the package and import statements , we then get down to the body of the file, which is where we add in a bunch of logic that actually kind of does something.
