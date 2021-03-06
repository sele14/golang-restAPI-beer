# Go REST API for Investment Portfolio
Add financial instruments to your portfolio! The rest-API supports GET, POST, and DELETE requests.

## Run

First, install Mux:
```go
go get -u github.com/gorilla/mux
```

Then, run the API:
```go
go run main.go
```

## Testing

Use an API testing tool like Postman and send a ```POST``` request and add an instrument like:

```json
{
	"ID" : "3",
	"Type" : "Cryptocurrency",
	"Name" : "BTC",
	"Price" : 27303.96,
	"Quantity" : 1,
}
```

And check the new contents by doing a ```GET``` request to see the updates.

Use the url http://127.0.0.1:8000/instruments.