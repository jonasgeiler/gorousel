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


## How run on each boot in Windows

I prefer letting gorousel update my wallpaper after each startup.  
To do this, open the **Registry Editor** and navigate to `HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows\CurrentVersion\Run`.  
There, all you have to do is add a new _String Value_ with the name `Gorousel` and the path to the gorousel executable as value.
