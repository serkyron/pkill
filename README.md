# pkill for Golang!

### Extremely simple, but cross-platform function to kill a process by it's process name
```go
import "github.com/SkyrisBactera/pkill"
// Kills chrome
output, err := pkill.Pkill("chrome")
if err != nil {
    fmt.Println(err)
}
fmt.Println(output)
```

**Note!** On Linux the underlying pkill command matches the process name you pass against a full command name. 