### Step 1
install "go"  
(use goproxy to make it working correctly if it is not.)  

### set GOPATH Variable

edit *`.bashrc`*  
*`
export GOPATH=$HOME/go
export PATH=$PATH:$GOROOT/bin:$GOPATH/bin  
`*

### install lf
`env CGO_ENABLED=0 go install -ldflags="-s -w" github.com/gokcehan/lf@latest`  

use command `lf` to start listFiles on current directory  

### Configuration
> 1. `mkdir -p ~/.config/lf`    
>`cp $GOPATH/src/github.com/gokcehan/lf/etc/lfrc.example ~/.config/lf/lfrc`  

> 2. `mkdir -p ~/.config/lf`  
`curl https://raw.githubusercontent.com/gokcehan/lf/master/etc/lfrc.example -o ~/.config/lf/lfrc`  

[Configuration Example](https://pkg.go.dev/github.com/gokcehan/lf#section-readme)  
