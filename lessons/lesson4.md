Examples in this lesson modifies existing string.

## String concatenation - `strcat`

The `strcat` function is used to append one string (source) at the end of another string (destination). It does the following:

1. Takes the destination string.
2. Finds the NULL character.
3. Copies the source string starting at the location of the NULL character of destination string.
4. Appends a NULL character to the destination string when all characters of the source string are copied to the destination string.

Here is an example:

```
char src[] = "Look Here";
char dest[40] = "Unimaginable";

strcat(dest, src);
printf("%s", dest); /* Output: UnimaginableLook Here */
```

Notice how it works. When `dest` is initialized with `char dest[40] = "Unimaginable";` there is a NULL character at the end. That's the starting point for the source string to be copied. When all characters of source string are copied to `dest`, a NULL character is appended.

Following properties which applied to `strcpy` are also applied to `strcat`:

1. The destination character array must be large enough to hold all characters of source, all characters of destination and a NULL character.
2. 
