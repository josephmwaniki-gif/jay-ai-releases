# Jay AI — Official Windows Releases

This public repository is for **compiled Jay AI release packages only**. The source code is maintained separately in a private repository.

## Downloading

When a release is published, download the Windows ZIP attached to that release. Extract the complete ZIP to a folder and run `JayAI.exe` from the extracted `JayAI` directory.

Keep the entire extracted folder together: the executable depends on files and folders bundled alongside it.

## Verify the package

Each release should include `SHA256SUMS.txt`. On Windows PowerShell, run the following in the folder containing the ZIP and checksum file:

```powershell
Get-FileHash .\JayAI-Windows-vX.Y.Z.zip -Algorithm SHA256
Get-Content .\SHA256SUMS.txt
```

Compare the computed hash with the published hash. A matching SHA-256 checksum detects accidental corruption; by itself, it does not prove who published the package.

## Important status

Jay AI is under active development. The current desktop build is a UI prototype. Online AI, voice, news, weather, the custom animated avatar, a per-user installer, and automatic updates are not yet complete. Do not assume automatic updates are available until a release explicitly documents them.

Never share GitHub tokens or passwords. Official update verification must be implemented before Jay installs updates automatically.
