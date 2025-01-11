# Dabing TeX files

## How to use

- in `postavy.tex` is dictionary of characters used in script using this structure
```python
{
    "alias": {
        "name": "Character Full Name",
        "constant": True                # default False, used to differentiate between characters that are constant or not on the front page
    }
}
```
- the script have to be put in `script.tex` using this format:
```tex
\characterLine{ALIAS}{TIME}{CHARACTERS_LINE}
```
where the values means this:
| Value | Desctiption |
| - | - |
| ALIAS | the defined alias in `postavy.tex` file |
| TIME | the timestamp in the episode/movie (can be empty) |
| CHARACTERS_LINE | the line that is being said by the mentioned character |