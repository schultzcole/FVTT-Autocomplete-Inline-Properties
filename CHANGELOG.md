# CHANGELOG

## [2.1.1] 2021-06-05

### FIXED

- Fixed an error that would occur on startup because the SW5e config was still referring to the old location of AIP constants
- Fixed an error that would occur on startup because a symbol was used before it had been initialized.

## [2.1.0] 2021-06-05

### ADDED

- Added compatibility with SW5e system. (Thanks Cyr-)

## [2.0.0] 2021-06-05

*Compatibility with 0.8.x*

### CHANGED

- [BREAKING] moved publicly accessible AIP properties from the global CONST and CONFIG into `game.modules.get("autocomplete-inline-properties").API`.

## [1.2.0] 2021-02-19

### ADDED

- Added pf1 support (thank you @MikauScekzen for the contribution!)
- Added support for `<textarea>` tags in addition to text `<input>` tags

## [1.1.0] 2021-02-17

### API

- Added several field configuration properties
  - `defaultPath`: sets the default path that will appear in the Autocompleter on initial load for the target field.
  - `DATA_MODE.OWNING_ACTOR_ROLL_DATA`: a new data mode which will get the roll data of the owning actor.
  - `customInlinePrefix`: a prefix that will be inserted in front of the final path in the target field when the Autocompleter is submitted.
  - `filteredKeys`: an array of keys which should not be displayed in the Autocompleter for the target field.

## [1.0.1] 2021-02-17

### FIXED

- Fix an issue which would cause `customDataGetter`s to not be as useful as they should have been.
- Fix an issue where an error would be thrown in circumstances where a data getter returned null or undefined

## [1.0.0] 2021-02-17

*Initial Release*
