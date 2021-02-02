# SharkDetector-MarketSentimentsMiner
Web API written in Go to mine social media comments and posts about a particular stock.

## Background
Since COVID started, more and more ordinary people turned into retail investors as a consequence of lockdown. Recent war between retailers and hedge funds sparked the interest of more social media users to start investing.
The market movement is heavily impacted by emotion especially when a larger portion of market fund comes from retailer without professional tools and experiences.
This leads to the importance of sentiment analysis in stock market prediction and the web api is created for mining tweets and comments about a stock. 

## How to use
### Build from source
Windows
``` sh 
$ set GOOS=windows 
$ set GOARCH=amd64
$ go build env_helper.go file_utils.go protocol.go router.go router_handler.go server.go twitter_handler.go validator.go yf_conversations_handler.go yf_conversations_handler_test.go
```
Linux: 
``` sh
$ set GOOS=linux
$ set GOARCH=amd64 
$ go build env_helper.go file_utils.go protocol.go router.go router_handler.go server.go twitter_handler.go validator.go yf_conversations_handler.go yf_conversations_handler_test.go
```
