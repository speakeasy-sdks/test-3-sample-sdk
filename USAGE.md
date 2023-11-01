<!-- Start SDK Example Usage -->


```go
package main

import (
	"context"
	test3samplesdk "github.com/speakeasy-sdks/test-3-sample-sdk"
	"log"
)

func main() {
	s := test3samplesdk.New()

	ctx := context.Background()
	res, err := s.Pets.CreatePets(ctx)
	if err != nil {
		log.Fatal(err)
	}

	if res.StatusCode == http.StatusOK {
		// handle response
	}
}

```
<!-- End SDK Example Usage -->