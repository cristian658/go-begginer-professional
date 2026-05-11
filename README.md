# From Beginner to Professional in Go

This repository contains the code examples and exercises for the book "From Beginner to Professional in Go".

## Getting Started

### How create a new Go module
To create a new Go module, you can use the following command in your terminal:
```bash
go mod init <module-name>
```
Replace `<module-name>` with the name you want for your module. This command will create a `go.mod` file in your current directory, which will be used to manage your module's dependencies.

Create file `main.go` and add the following code:
```go
package main
import "fmt"
func main() {
    fmt.Println("Hello, World!")
}
```
### How to run the code
To run the code, you can use the following command in your terminal:
```bash
go run main.go
```
This command will compile and execute the `main.go` file, and you should see the output:
```bash
Hello, World!
```

### What is mod tidy 

The `go mod tidy` command is used to clean up the `go.mod` file and the `go.sum` file by removing any dependencies that are no longer needed. It also adds any missing dependencies that are required by the code in your module. This helps to ensure that your module's dependencies are accurate and up-to-date. You can run this command in your terminal with:
```bash
go mod tidy
```
This will analyze your code and update the `go.mod` and `go.sum` files accordingly. It's a good practice to run `go mod tidy` regularly to keep your module's dependencies clean and organized.