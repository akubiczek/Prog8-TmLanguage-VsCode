# Prog8 language syntax highlighting

This project is a syntax definition for the Prog8 programming language. It enables syntax highlighting in editors like Visual Studio Code, Sublime, IntelliJ IDEA, etc. 
In addition to general syntax definition, you can find here ready to use extensions for:

1. Visual Studio Code
2. Sublime 3

The project is still far from being perfect - your contribution is warmly welcomed.

## Extension installation

Instructions on installing extensions are in a respective extension's folder.

## Contribution workflow

Syntax definition is made using the Iro tool https://eeyo.io/iro/documentation/ using Rion Object Notation. This format is straightforward to understand, develop, and maintain. The source file is `src/Prog8.iro`.

### Step 1 - upgrade general syntax definitions

1. Open `./src/Prog8.iro` in https://eeyo.io/iro/
2. Edit, test, and save `./src/Prog8.iro` file
3. From the Iro tool, export to Textmate XML file and save as `./src/Prog8.tmLanguage.xml`

### Step 2 - prepare Visual Studio Code extension

1. Convert Textmate XML to Textmate JSON and save it as `./visualstudiocode/Prog8/syntaxes/Prog8.tmLanguage.json` (you can use `TextMate Languages` Visual Studio Code extension to convert)
2. Could you manualy replace `"name": "prog8",` with `"name": "Prog8",` in the `Prog8.tmLanguage.json` please? :)

### Step 3 - prepare Sublime 3 extension

1. Copy `./src/Prog8.tmLanguage.xml` to `./sublime3/Prog8/support/Prog8.tmLanguage` (without .xml file name extension!)
