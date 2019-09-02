
```js no-beautify
"" + 1 + 0 = "10" // (1)
"" - 1 + 0 = -1 // (2)
true + false = 1
6 / "3" = 2
"2" * "3" = 6
4 + 5 + "px" = "9px"
"$" + 4 + 5 = "$45"
"4" - 2 = 2
"4px" - 2 = NaN
7 / 0 = Infinity
" -9  " + 5 = " -9  5" // (3)
" -9  " - 5 = -14 // (4)
null + 1 = 1 // (5)
undefined + 1 = NaN // (6)
" \t \n" - 2 = -2 // (7)
```

<<<<<<< HEAD
1. Додавання пустого рядка `""` до `1` перетворює число `1` на рядок: `"" + 1 = "1"`; далі ми маємо `"1" + 0`, в якому застосовується те ж саме правило.
2. Віднімання `-` (як і більшість математичних операцій) працює тільки з числами, воно перетворює порожній рядок `""` на `0`.
3. Додавання з рядком додає число `5` до рядка.
4. Віднімання завжди перетворює рядки на числа, тому рядок `"  -9  "` перетвориться на число `-9` (ігноруючи пробіли навколо нього).
5. `null` стає `0` після числового перетворення.
6. `undefined` стає `NaN` після числового перетворення.
=======
1. The addition with a string `"" + 1` converts `1` to a string: `"" + 1 = "1"`, and then we have `"1" + 0`, the same rule is applied.
2. The subtraction `-` (like most math operations) only works with numbers, it converts an empty string `""` to `0`.
3. The addition with a string appends the number `5` to the string.
4. The subtraction always converts to numbers, so it makes `"  -9  "` a number `-9` (ignoring spaces around it).
5. `null` becomes `0` after the numeric conversion.
6. `undefined` becomes `NaN` after the numeric conversion.
7. Space characters, are trimmed off string start and end when a string is converted to a number. Here the whole string consists of space characters, such as `\t`, `\n` and a "regular" space between them. So, similarly to an empty string, it becomes `0`.
>>>>>>> c4d1987ebc470b30c234dbde6fac6e77b7509927
