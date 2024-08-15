# Value and Variable in OCaml

Value in programming is a data representation such number, boolean, fraction (float) and words (a.k.a string). 

```ocaml
1;; (* number *)
1.23;; (* fractional number *)
true;; (* boolean notation *)
"OCaml";; (* string *)
```

Why there a representation ? because every value will stored in memory as uniform in bytes, so this representation giving a tagging how to program should treat the data. 

This type of representation is called type system. Speaking of type system, OCaml treat type statically. Each type of value that assigned to variable can not be change after declared or initialize.

Variable is a way to storing value in a name for later to be used in operation or storing a result of operation. Think a pouch that have name on it, then you put thing inside. So, when you recall the item you can fetch conviniently by recall the pouch name.

In depth view, variable is abstracting how to store and load data from memory without much hassle.

```ocaml
let me = "Adashino" ^ "Nayuta" ;;

print_endline name;;
```
Look at code above. The code is explain about declaring variable (using `let`) with name `me` and storing value from concating string (`"Adashino" ^ "Nayuta"`). The value will accessible as we type the name (`me`) into operation. 

One operation here is invoking function `print_endline` with argument variable (`me`), the argument will replaced with real value that stored in that variable. So, here the process of storing and loading value from memory similary with variable in basic algebra and calling people with its name.

In low-level, storing and loading value with need dealing with hex address such (`0x00004321` so forth) and dealing with register to store address and value. I not much know the detail for instruction, at least the big picture pretty much like that.

## Snippet

- Declaring variable :
  - `let [variable name] = [value];;` (e.g `let namae = "Sayaka";;`)
  - `let [variable name]:[type] = [value];;` (e.g `let fullname : string = "Saeki Sayaka";;`)

