# styled-printf
[![Hex.pm](https://img.shields.io/hexpm/l/plug.svg?maxAge=2592000&style=flat-square)](https://github.com/bvanhoekelen/terminal-style/blob/master/LICENSE)

Do you want to add some styles 🎨 to the output of your bash **printf** commands? Use this custom script and make the output of that **printf** look fanzy :bowtie: 

## How to use

The `styled-printf` command is like `printf` (in fact it's a function wrapping `printf`) that accepts 3 extra options + value:

| Option | Description | Values |
| ------ | --- | --- |
| `-s` \| `--style` | Text formatting | `normal` \| `bold` \| `dim` \| `italics` \| `underline` \|<br /> `blink` \| `reverse` \| `hidden` \| `password` |
| `-c` \| `--color` | Text color | `default` \| `white` \| `black` \| `red` \| `green` \|<br /> `yellow` \| `blue` \| `magenta` \| `cyan` \| `gray` \|<br /> `light-red` \| `light-green` \| `light-yellow` \|<br /> `light-blue` \| `light-magenta` \| `light-cyan` \|<br /> `light-gray` \| <br /><br /> or a number between`0` and `256` | |
| `-b` \| `--background-color` | Background color | `default` \| `white` \| `black` \| `red` \| `green` \|<br /> `yellow` \| `blue` \| `magenta` \| `cyan` \| `gray` \|<br /> `light-red` \| `light-green` \| `light-yellow` \|<br /> `light-blue` \| `light-magenta` \| `light-cyan` \|<br /> `light-gray` \| <br /><br /> or a number between`0` and `256` | |

### Example
```Shell
styled-printf -s bold -c red -b blue "%s\n" "This text is bold, red and has a blue background"
```
