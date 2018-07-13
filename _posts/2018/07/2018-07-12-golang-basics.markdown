$cat main.go 
// all runnable go programs must have a main package and one main function
package main
import "fmt"

func main() {
	fmt.Println("Hellooooo")
}


$go build

$ls -lrt
total 4088
-rw-r--r--  1 aru  staff      144 Jul 12 21:08 main.go
-rwxr-xr-x  1 aru  staff  2085008 Jul 12 21:09 hello

$/hello 
Hellooooo
 
directly running it
$go run main.go
Hellooooo

# format it and write the file
# gofmt tools
gofmt -w main.go



$ cat userarg.go 
package main

import ( 
	"fmt"
	"os"
)

func main() {
	if len(os.Args) > 1 {
		fmt.Println(os.Args[1])
	} else {
		fmt.Println("Hello, I am Gopher")
	}
}

$ go run userarg.go  first-argument
first-argument
