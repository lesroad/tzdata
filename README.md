# tzdata
A uncompressed zip file of IANA time zone database files, can be used to set timezone in go program.

# Example
``` // rootPath is the workdir or some absolute path
os.Setenv("ZONEINFO", rootPath)
l, _ := time.LoadLocation("Asia/Shanghai")
fmt.Println(time.Now().In(l)) // 2019-05-17 15:57:43.0785088 +0800 CST 
```
