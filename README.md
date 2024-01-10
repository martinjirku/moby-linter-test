# Linters

Just testing misspell linting. 

- Install linter: `curl -sSfL https://raw.githubusercontent.com/golangci/golangci-lint/master/install.sh | sh -s -- -b $(go env GOPATH)/bin v1.55.2`
- Run: `golangci-lint run`

```sh
main.go:6:37: `cancelled` is a misspelling of `canceled` (misspell)
  // this is misspelled comment for cancelled
                                    ^
main.go:7:3: `cancelled` is a misspelling of `canceled` (misspell)
  cancelled := true
  ^
main.go:8:47: `cancelled` is a misspelling of `canceled` (misspell)
  fmt.Printf("This is misspelled word: %t\n", cancelled)
                                              ^
```
