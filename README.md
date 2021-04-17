# Gorousel

A stupidly simple wallpaper carousel program.  
Just build the binary and then add a cronjob to run on every login.  
Works like a charm!

## Run

Clone this repo and then run:
```
go run .
```

## Build Binary

Just run:
```
go build
```

To build an optimized binary on Windows:
```
go build -ldflags "-H windowsgui -s -w"
```