# clidna
Dead simple IDNA encode / decode  command line tool


Will encode / decode names from / to IDNA


## Examples

Using arguments from the command line:

```console
shell:~$ idna thé-ou-café.com ☕.com
xn--th-ou-caf-c4ah.com
xn--53h.com

shell:~$ idna xn--apro-cpa.fr xn--xj8h
apéro.fr
🍺
```

… or using the standard input (will split on spaces)

```console
shell:~$ echo made-with-❤.org xn--fi8h.garden | idna
xn--made-with--lo3g.org
🍅.garden

```

This single script is using python3 and needs the `idna` (`python3-idna`) module to properly handle some conversions (will still work without it)
