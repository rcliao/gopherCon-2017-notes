# Go Anti-Patterns

https://gist.github.com/freeformz/4746274

## Go's Design Principles

* Orthogonality
* Simplicity
* Readabbility

### Orthogonality

Pieces are independent from each other.

Example: io.Reader and io.Writer

### Simplicity

Reduce features from other languages for example.

### Readability


## Go Anti-Patterns

### Tiny Package Syndrone

Lots of packages each containing a single file as example.

> Do it with larger package or group them by types.

### Premature Exportation

Everything is exposed.

> E.g. exposing internal type

Make some packages as "internal" package

> Client cannot use internal package from other package.

### Package `util`

Package name "util" doesn't say anything about package

> Name of package should describe its purpose not its content.

### Config/Option Structs

Don't use a big "config" struct to contain all the input parameter. 

> Make the input parameter in the method signature as close as what it needs.

### Pointer all the things

STOPS!

When you pass a pointer to a function, you are passing the ownership of the var
to the function.

### Context.Value

It's a trap!

> There are other way to share value through out the request chain.

### Asynchronous API

See http apckage and buffio.Scanner type

User channel internally and expose synchrouslly

### IF then else pattern

* Handle error early and return early
* Keep the indentation level as low as possibble

### Interface all the things

The bigger the interface, the weaker the abstraction.

### Naked return values

### Empty `interface{}`

User the interface for unknown data; otherwise don't use it.


