# SampleGoCommands

This is a list of useful GO commands.

- The -u flag adds information about available upgrades. When the latest version of a given module is newer than the current one, list -u sets the Module's Update field to information about the newer module. 
  ```
  go list -u -m all
  go list -m -versions github.com/TsubasaEX/SampleGoModPkg/v2
  go list -m -u -json all
  ```
- The commands list current used versions
   ```
  go list -u -m all
  go list -m -json all
  ```
- This command deletes the cache downloaded along with unpacked code dependencies.
   ```
  go clean -modcache
  ```
- Tidy makes sure go.mod matches the source code in the module. It adds any missing modules necessary to build the current module's packages and dependencies, and it removes unused modules that don't provide any relevant packages. It also adds any missing entries to go.sum and removes any unnecessary ones. The -v flag causes tidy to print information about removed modules to standard error.
   ```
  go mod tidy
  go mod tidy -v 
  ```
  
References
- VSCODE
  - Extensions
    - **Language**
      - GO 
    - **Git**
      - Git History
      - GitLens
    - **Auto Completed Code**
      - TabNine
    - **Database (SQL + NoSQL)**
      - SQl Server Client(mssql)
      - Database Client
    - **Remote SSH Debug**
      - Remote SSH
    - **Reveal current file in Explorer**
      - Reveal
    - **Show External Libraris**
      - Go Mod Explorer
  - Commands
    - **Prompt Command Line**
      - Ctrl + Shift + P 
    - **Fold ALL Code Block**
      - Ctrl + Shift + K + 0
    - **Fold ALL Code To Level 1**
      - Ctrl + Shift + K + 1
    - **Fold ALL Code To Level 2**
      - Ctrl + Shift + K + 2
    - **UnFold ALL Code Block**
      - Ctrl + Shift + K + J    

