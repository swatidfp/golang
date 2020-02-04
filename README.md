# Golang
Very Basic implementation of Golang with Gokit. Gokit is a toolkit to build microservices in Golang. Learn more about [Gokit](https://gokit.io/)
## Installation
Optional but recommended 
``` 
$ sudo apt-get update
$ sudo apt-get -y upgrade
```
Installing Golang
``` 
$ wget https://dl.google.com/go/go1.13.3.linux-amd64.tar.gz
$ sudo mv go /usr/local
```
Setting up workspace
```
$ mkdir $HOME/go
$ sudo nano ~/.profile
# In the end add these lines 
export GOROOT=/usr/local/go # Optional - where Go package is installed on your system (Set this if you chose an alternate installation location for Go)
export GOPATH=$HOME/go # location of your work directory
export PATH=$PATH:$GOPATH/bin # variable to access go binary system wide
```
Now save the file and reload it via :
```
source ~/.profile
```
 ## Testing Installation
 Check if Go is installed by checking version
 ```
 go version
 ```
 Create a Hello world (Sample project)
 ```
 $ mkdir -p $GOPATH/src/github.com/blah
 $ mkdir $GOPATH/src/github.com/blah/hello
 $ touch $GOPATH/src/github.com/blah/hello/hello.go
 ```
 Copy this code in hello.go
 ```
package main
import "fmt"
func main() {
    fmt.Printf("Hello, world\n")
}
```
Save the file. Now time to create executable file and run it
```
$ go install github.com/blah/hello # this will install the file (create binary executable file)
$ cd $GOPATH/bin
$ ./blah # o/p Hello, world

```

 