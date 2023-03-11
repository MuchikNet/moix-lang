# MOIX Language 

```
[ M ]orphisms
[ O ]bjects
[ I ]dentity and
[ X ] is life
```


## Syntax

[hello.cat](/examples/hello.cat)
```haskell
cat Main
    use HelloWorld as HW
    mor main:
        HW.say

cat HelloWorld
    use IO
    ob Message: IO.in -- default: Raw
    mor say: Message -> IO.out
```

* `cat` => Category
    * `use` => Use a category
* `mor` => Morphism
    * `->` or `<-` => Direction
* `ob` => Object
* `id` => Identity
* `X` => Names start with a capital letter
* `--` => Comment line
* Category`.`Morphism => Use a morphism


## Categories

#### Types of data

* `Raw` - Input data (Unicode)
* `Num` - Numbers
* `Str` - Strings
* `[]` - Array
* `()` - List
* `{}` - Group

#### IO - Input / Output

* `.in` - Input
* `.out` - Output


## License

```
GNU GENERAL PUBLIC LICENSE
Version 3, 29 June 2007
```
