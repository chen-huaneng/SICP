---
aliases: 
tags: ""
source: 
created: 2023-06-30 23:01
---

[中文版本|The original text](https://zhuanlan.zhihu.com/p/405246479)

以下为原文翻译转载，如果侵权请联系我删除  

The following is a translation of the original text, if there is infringement, please contact me to delete

1. Download [ChezScheme](https://github.com/cisco/ChezScheme)
2. Default install route:


```json
C:\Program Files\Chez Scheme 9.5.4\bin\ta6nt (64-bit, windows)  
C:\Program Files (x86)\Chez Scheme 9.5.4\bin\ti3nt (32-bit, windows)
```

3. Add environmental path: PATH = `C:\Program Files\Chez Scheme 9.5.4\bin\ta6nt`
4. Install VSCode Extension: vscode-scheme, Code Runner  
5. Modify VSCode settings (VSCode -> Settings (`Ctrl` + `,`) -> Open Settings)

```json
Add: "code-runner.runInTerminal": true  
Add: "code-runner.executorMapByFileExtension": {".ss": "scheme"}  
Modify: "code-runner.executorMap": "scheme": "csi -script", -> "scheme": "scheme",
```

6. Restart VSCode
7. New file `hello-scheme.ss`
```scheme
(display "Hello Scheme!")
(exit)
```

8. Run `Ctrl` + `Alt` + `N`

```cmd
C:>scheme "C:\hello-schema.ss"
Chez Scheme Version 9.5.4
Copyright 1984-2020 Cisco Systems, Inc.

Hello Scheme!
```


