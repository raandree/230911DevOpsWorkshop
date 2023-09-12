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
- [Customize your VS Code setup for a project, or for a language](https://www.roboleary.net/vscode/2020/09/17/vscode-workspace-settings.html#:~:text=Typically%2C%20a%20VS%20Code%20%E2%80%9Cworkspace%E2%80%9D%20is%20just%20your,and%20they%20are%20stored%20locally%20in%20%3C%3Cproject%20folder%3E%3E%2F.vscode%2Fsettings.json.)
asdasd
Branch models

[Trunk based development](https://trunkbaseddevelopment.com/)
[Git Flow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)


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
