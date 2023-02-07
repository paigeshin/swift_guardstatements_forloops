# swift_guardstatements_forloops

```swift
// You can use the 'guard' statement to...

for string in strings {
    // ...continue an iteration
    guard shouldProcess(string) else {
        continue
    }
    
    // ...or break it
    guard !shouldBreak(for: string) else {
        break
    }
    
    // ...or return
    guard !shouldReturn(for: string) else {
        return
    }
    
    // ..or throw an error
    guard string.isValid else {
        throw StringError.invalid(string)
    }
    
    // ...or exit the program
    guard !shouldExit(for: string) else {
        exit(1)
    }
}
```
