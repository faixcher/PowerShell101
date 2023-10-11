
``` powershell
Get-ChildItem -File -Hidden -ErrorAction SilentlyContinue

output >> list hidden file 

Get-Childitem -Directory -Hidden -Filter ".pdf"

output >> list only .pdf 
```

count word of file 
```powershell
Get-Content hello.txt | Measure-Object -Word

output >> 500 word 
```

look content in file with INDEX 
```powershell
(Get-Content hello.txt)[5555,54444]

output >> fais , saleng 
```

look content in file with STRING
```powershell
get-content hello.txt | Select-String  -Pattern 'fais'

output >> fais 
```

