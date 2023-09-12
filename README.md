## 1.1. Additional Agenda

-	Functions and modules
-	File copy in a pipeline to azure file share
-	Connect to ExOnline
-	CRON jobs
-	Pipeline Parameters

## 1.2. Additional Resources

- [PowerShellTraining](https://github.com/raandree/PowerShellTraining)
- [Markdown Guide](https://www.markdownguide.org/)
  - [Pandoc](https://pandoc.org/)

```powershell
    param(
        [Parameter(Mandatory, ValueFromPipeline)]
        [ValidateScript( { Test-Path -Path $_ -PathType Container })]
        [string[]]$Path,
                
        [ValidateRange(1, [long]::MaxValue)]
        [long]$MaxSize = 100KB,
        
        [switch]$AddSummary
    )
```
