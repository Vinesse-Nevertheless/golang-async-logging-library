# Logging Library with Go

In this project, you'll use Go's concurrency tools to build a fully asynchronous logging package. You'll start with a simple, synchronous logger and add new features which allow log messages to be stored with minimal impact on the performance of your application.

## Setup
Setup your local environment for this project. We'll walk you through everything you need to know to setup your local instance, and to access the code you'll be using for this project.

## Writing Asynchronous Log Entries
In this module, you'll add the primary functionality of the logger. This includes support for thread-safe, asynchronous writes to the log and concurrent error handling.

## Shutting Down the Log
Eventually, almost all applications need to exit and they should do so gracefully. In this module, you'll add some additional capabilities to the asynchronous logging package that will allow the log to be shut down while ensuring that no pending messages are lost.


## To use the test runner:

* navigate into the ./cmd directory
* if run with the defaults (`go run .`), the application will run in asynchronous mode and write it's output directly to the shell
    * the `-out` flag allows a destination file to be specified
    * the `-async` flag determines if the logger will asynchronously or not. It is async by default, which will not work properly in the application's initial condition.

## To run the tests

* use the `go test` command from the command line
* to focus on a specific test, use the `-run` flag followed by a pattern that matches the test name
    * e.g. `go test -run MessageChannel` will run the first test of the first module
* all tests for a given module can be run by passing the module identifier to the `-run` command
    * e.g. `go test -v -run Module1`
