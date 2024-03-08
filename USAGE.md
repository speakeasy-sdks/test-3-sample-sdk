<!-- Start SDK Example Usage [usage] -->
```go
package main

import (
	"context"
	test3samplesdk "github.com/speakeasy-sdks/test-3-sample-sdk"
	"github.com/speakeasy-sdks/test-3-sample-sdk/pkg/models/shared"
	"log"
)

func main() {
	s := test3samplesdk.New()

	ctx := context.Background()
	res, err := s.Pets.CreatePets(ctx, shared.Pet{
		ID:   596804,
		Name: "<value>",
	})
	if err != nil {
		log.Fatal(err)
	}
	if res != nil {
		// handle response
	}
}

```
<!-- End SDK Example Usage [usage] -->