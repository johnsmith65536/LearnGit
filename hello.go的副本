package main

import "fmt"

func queryString(S string, N int) bool {
    
    var n int = len(S)
    if N>(n+1)*n/2{
    	return false
    }
    var vis[2000000] bool
    for i:=0;i<n;i++{
    	var sum int = 0
    	for j:=i;j<n;j++{
    		sum=sum*2+int(S[j])-int('0') 
    		if sum>N{
    			break
    		}
    		vis[sum]=true
    	}
    }
    for i:=1;i<=N;i++{
    	if(!vis[i]){
    		return false
    	}
    }
    return true;
}

func main(){
	fmt.Println(queryString("0110",4))
}