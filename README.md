# CoApp scripts for OVR via NuGET

Use this package to create NuGet packages that add Oculus VR SDK to your
Visual Studio projects!

## Updating OVR version.
First, download new binary packages from Oculus VR website.
```bash
$ vi ovr.autopkg  # change version and directories defines to match
$ git commit -m "Updated libOVR version to vX.XXXX.XXXX"
```

## Building OVR NuGet packages.
In Powershell
```bash
> Write-NuGetPackage .\OVR.autopkg
```

## Installing CoApp NuGet helper scripts.
In administrator PowerShell:
```
> Set-ExecutionPolicy -Scope CurrentUser RemoteSigned
```

In normal PowerShell:
```
> Update-CoAppTools -KillPowershells
```
