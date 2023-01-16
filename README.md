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
