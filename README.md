# prog8-lang syntax highlighting

This is an Visual Studio Code extension to enable syntax highlighting for Prog8 language.

This is also a generic textmate syntax highlighting to use in other IDEs.

The grammar file may be far from being perfect - your contribution is warmly welcome.

## Workflow

1. Open `src/prog8.iro` in https://eeyo.io/iro/
2. Edit & export to Textmate XML file `src/prog8.textmate.xml`
3. Convert Textmate XML to Textmate JSON `syntaxes/prog8.tmLanguage.json` (you can use `TextMate Languages` extension for VSC)

## Install in Visual Studio Code

1. Make a new folder in VSC `./extensions/` and name it `prog8`
2. Copy `package.json`, `language-configuration.json` and `syntaxes/` folder into the new `prog8` folder
3. Restart Visual Studio Code
