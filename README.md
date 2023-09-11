# 1. DevOps Workshop (11.09.2023)
- [1. DevOps Workshop (11.09.2023)](#1-devops-workshop-11092023)
  - [1.1. Additioanl Agenda](#11-additioanl-agenda)
  - [1.2. Additioanl Resources](#12-additioanl-resources)

## 1.1. Additioanl Agenda

-	Functions and modules
-	File copy in a pipeline to azure file share
-	Connect to ExOnline
-	CRON jobs
-	Pipeline Parameters

## 1.2. Additioanl Resources

- [PowerShellTraining](https://github.com/raandree/PowerShellTraining)
- [Markdown Guide](https://www.markdownguide.org/).
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