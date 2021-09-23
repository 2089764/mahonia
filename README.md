# mahonia
character-set conversion library implemented in Go.

Mahonia is a character-set conversion library implemented in Go. All data is compiled into the executable; it doesn't need any external data files.

#
based on http://code.google.com/p/mahonia/
fork	https://github.com/Tang-RoseChild/mahonia

# example
```
package main
import (
	"fmt"
	import "https://github.com/2089764/mahonia"
)
func main(){
  fmt.Println(GBK2UTF8("hello,世界"))  
}

//GBK2UTF8 GBK编码转换为UTF8
//converts a  string from UTF-8 to gbk encoding.
func GBK2UTF8(s string) (string, bool) {
	dec := mahonia.NewDecoder("gbk")
	return dec.ConvertStringOK(s)
}
```