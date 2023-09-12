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
- [AutomatedLab](https://automatedlab.org/en/latest/)

## Coding guidelines
- [THE CURIOUS CASE OF $NULL](https://evotec.xyz/the-curious-case-of-null-should-be-on-the-left-side-of-equality-comparisons-psscriptanalyzer/#:~:text=The%20only%20way%20to%20reliably,cast%20to%20other%20scalar%20types).
- [PSScriptAnalyzer](https://github.com/PowerShell/PSScriptAnalyzer)



One settings file per VSCode workspace (settings.json)



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
