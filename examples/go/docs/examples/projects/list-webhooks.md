# Projects Examples

## ListWebhooks

```go
    package appwrite-listwebhooks

    import (
        "fmt"
        "os"
        "github.com/appwrite/go-sdk"
    )

    func main() {
        // Create a Client
        var clt := appwrite.Client{}

        // Set Client required headers
        clt.SetProject("")

        // Create a new Projects service passing Client
        var srv := appwrite.Projects{
            client: &clt
        }

        // Call ListWebhooks method and handle results
        var res, err := srv.ListWebhooks("[PROJECT_ID]")
        if err != nil {
            panic(err)
        }

        fmt.Println(res)
    }
```