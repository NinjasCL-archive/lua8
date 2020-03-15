# Lua Oito (Lua 8)

This is a fork of [lua v5.3.5](https://github.com/lua/lua/tree/v5.3) with some [power patches](http://lua-users.org/wiki/LuaPowerPatches) to save tokens in [fantasy consoles/computers](https://github.com/paladin-t/fantasy). Like [TIC-80](https://github.com/nesbox/TIC-80).

## Included Patches

These are some of the patches included.

## [Perl Style Numerals](https://hoelz.ro/projects/lua-power-patches)

This patch allows you to insert underscores
arbitrarily into numbers, like you can in Perl.
This allows you to type `1_000_000` for 1 million.
Based on `perl-numbers.patch` by _Hoelz_.

## [Compound Assignment Operators](http://lua-users.org/files/wiki_insecure/power_patches/5.4/plusequals-5.4.patch)

Allows statements like `"object.counter += 2"`. Adds shift and bitwise operators `(<<=, >>=, &=, |=, and ^=)` to the previously implemented `+=, -=, *=, and /=.`. Based on `plusequals-5.4.patch` By _Dave Hayden_ (<dave@panic.com>) and _SvenOlsen_.

## iOS Compatible

iOS is not an _ISO C_ platform, which is what Lua commits to. So special changes were added to `loslib.c` to be compatible with this operating system.

You need to set ON the `IOS` flag.

Thanks to [@jet082](https://github.com/jet082)
See https://github.com/libretro/TIC-80/issues/2
