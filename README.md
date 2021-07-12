# styled-printf
[![Hex.pm](https://img.shields.io/hexpm/l/plug.svg?maxAge=2592000&style=flat-square)](https://github.com/bvanhoekelen/terminal-style/blob/master/LICENSE)
[![npm](https://img.shields.io/npm/v/npm-auto-version.svg?maxAge=2592000)](https://www.npmjs.com/package/https://www.npmjs.com/package/styled-printf)


Do you want to add some styles 🎨 to the output of your bash **printf** commands? Use this custom script and make the output of that **printf** look fanzy :bowtie: 

## How install

Using Yarn
```Shell
yarn add styled-printf
```

Using NPM:
```Shell
npm i styled-printf
```

## How to use

The `styled-printf` command is like `printf` (in fact it's a function wrapping `printf`) that allows you to easily set the text styling, color and background color for the output.

### Usage:
```Shell
styled-printf [-s <text format>] [--style <text format>] [-c <color>] [--color <color>] [-b <color>] [-background-color <color>] format [argument]
```

### Options:
| Option | Description | Values |
| ------ | --- | --- |
| `-s` \| `--style` | Text formatting | `normal` \| `bold` \| `dim` \| `italics` \| `underline` \|<br /> `blink` \| `reverse` \| `hidden` \| `password` |
| `-c` \| `--color` | Text color | `default` \| `white` \| `black` \| `red` \| `green` \|<br /> `yellow` \| `blue` \| `magenta` \| `cyan` \| `gray` \|<br /> `light-red` \| `light-green` \| `light-yellow` \|<br /> `light-blue` \| `light-magenta` \| `light-cyan` \|<br /> `light-gray` \| <br /><br /> or a number between`0` and `256` | |
| `-b` \| `--background-color` | Background color | `default` \| `white` \| `black` \| `red` \| `green` \|<br /> `yellow` \| `blue` \| `magenta` \| `cyan` \| `gray` \|<br /> `light-red` \| `light-green` \| `light-yellow` \|<br /> `light-blue` \| `light-magenta` \| `light-cyan` \|<br /> `light-gray` \| <br /><br /> or a number between`0` and `256` | |

### Example
```Shell
styled-printf -s bold -c blue -b yellow "%s\n" "This text is bold, red and has a blue background"
```

<img src="https://github.com/alvarezmauro/styled-printf/blob/main/assets/example-output-01.png" width=450 alt="styled-printf output: text 'This text is bold, red and has a blue background' in blue color, bold and yellow background">

### Other flags:
| `-h` \| `--help` | Display the help documentation |
| ------- | ------- |
| `-t` \| `--test` | Test all the different styles in your bash terminal |
