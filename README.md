# Commits Format

## Under Development

Currently under early development stage therefore any api can and will change

## About

Commits format created as standard that describe formats of commit messages using config file.

### Easy create format

It's easy to create formats of commit message for repository by maintainers by simply creating config file in
root folder of repository.

### Easy consume format

It's easy to consume formats by using tools that consume config file and helps to
create commit messages that follow format.

### Easy examples

It's easy to create examples of commit messages that follow format by simply changing values of variables and receive
multiple examples of commit messages that follow format.

## How it helps maintainers

Maintainers can formalize format of commit messages and provide it to developers by simply creating config file in root

### Format main parts

Format mainly consist of two parts:

- Variables - any values than need to be used in template of commit message
- Template - object that describe actual format string of commit message and can use variables to create commit message

Values of variables can be provided directly in config file or provided by developer using tool that consume config
file.

### Multiple formats

Since it's possible to have different formats for different commits in same repository it's possible to have multiple
formats in same config file.

## How it helps developers

By using tool that consume config file developers can easily create commit message that follow format of commit
messages.

### What kind of tools

Tool can be cli tool or browser extension or IDE extension or any other tool that can consume config file and way
to create commit message.

## Config file

Config file is json or json5 file that describe format of commit messages.

See [JSON5](https://json5.org/) for more information about json5 format.

Config file placed in root folder of repository and can be named one of the following:

- `commits-format.json`
- `commits-format.json5`
- `.commits-format.json`
- `.commits-format.json5`

It's also possible to have both json and json5 config files in same repository and use both of them to provide wider
tool support, but it's name must be different only by extension.

For example:

- `commits-format.json` and `commits-format.json5`
- `.commits-format.json` and `.commits-format.json5`

### Json schema

Config file must be valid against json schema of respective version of commits format.

See [JSON Schema](https://json-schema.org/) for more information about json schema.

Json schemas can be found in [schemas](./src/schemas) folder of this repository.