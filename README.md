# DotnetPublishErrorDemo
Demonstrates the error that occurs when using solution filters with @ characters in the path name.

Issue https://github.com/dotnet/sdk/issues/29141

### Remarks
- normally the Folder with the @ in the name is NOT part of the repo. It gets created by Jenkins as working directory. Then the code is cloned in that working directory. But for the sake of the example I added that folder to the git repo.
- You can ignore all the actual code in the repo. I just called File/New/Project twice to simulate a need for a solution filter. But all that is really relevant are the publish.ps1 and the SomeWebApplication.slnf with the corresponding WebApplications.sln

### Steps
1. clone the repo
2. execute publish.ps1 (or the dotnet publish command that is inside of it)
3. You will get the error
