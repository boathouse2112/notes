# Feature addtions

## Calculating match statistics from the command line

Ticket #1718
[https://sourceforge.net/p/omegat/feature-requests/1718/]

Currently `Project` and `Individual File` statistics can be calculated using:
```
java -jar /Applications/OmegaT.app/Contents/Java/OmegaT.jar mode=console-stats <PROJECT_DIR>
```

It would be nice if `Tools > Match Statistics` could be calculated using the same process

## Task list

- [ ] Ask if I should work on this or wait until CLI improvement
- [ ] Find where `mode=console-stats` is in the source files
- [ ] Find where console stats are calculated in the tool window
  - [ ] How are the 2 different?
- [ ] Find where `Match Statistics` are calculated in the tool window

## Mailing list -- command line improvement discussion

[https://sourceforge.net/p/omegat/mailman/omegat-development/thread/9902ff05-8b58-4739-950e-75b9ec673df0%40northside.tokyo/#msg58728618]

Hiroshi:
  Propose CLI structure:
    OmegaT <COMMAND> <SUB_COMMAND> <OPTIONS> <ARGUMENTS>

There are localization-bundle considerations I don't understand.

## Argument parsing

In `main`, the `Map<String, String> PARAMS` is filled with `CLIParameters.parseArgs(args)`

## Console Stats

In `Main.java`, method `runConsoleStats()`

## Match stats
File `core/statistics/MatchStatCounts.java`


