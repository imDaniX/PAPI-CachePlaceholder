# Archived - moved to [UtilityHooks](https://github.com/imDaniX/UtilityHooks)

# CachePlaceholder
A simple placeholder expansion that caches the result of other placeholders for desired period.

Might be useful when you have some resource-intensive placeholders that are called frequently, but it's not that 
important to keep those somewhat up-to-date.
## Usage
To install the expansion place it into the `plugins/PlaceholderAPI/expansions` folder.
### Format
The format is simple: `%cache_{cooldown}_{another_placeholder}%`

If given cooldown is equal to 0, the placeholder will return latest cached value.
Cached results are cleared once player leaves the server.

Example:
* `%statistic_time_played%` with 10 seconds delay: `%cache_10_statistic_time_played%`
* `%vault_eco_balance%` cache once: `%cache_0_vault_eco_balance%`
