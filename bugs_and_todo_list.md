# todo
* find all configdir folders yourself instead of prompting for the user's steamid. this will remove the need for a setup file.
* account for double quotes in an alias
* provide user with dump binds for autoexec:
 * // condump
 * bind [ +dump
 * alias +dump "clear; status"
 * alias -dump "condump"
 * bind ] "exec results"
* error check for malformed records in condump. if condump fails to export accurately, skip the record and continue
* account for other division names. unexpected names are exported to $configdir\log.txt
* handle special characters in the alias
* test if anti virus software cares about the batch, or that it calls powershell without using the profile's execution policy

# bugs
* (on valve) the content in console is not reliably sent to the export via the "condump" command. errors include standard characters in aliases being truncated, double quotes surrounding aliases, ect. tweeted @csgo_dev, no response
* if there is only one user in the condump, $allaliases.Length returns the length (in characters) of the single alias, not how many aliases there are

