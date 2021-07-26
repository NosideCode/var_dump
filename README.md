
# var_dump
PHP's var_dump function for JavaScript.

```js
var_dump({
    string: "hello",
    array: ["world!"],
    object: {
        subkey: [1, 2, {deep: "nested"}],
        empty: {}
    },
    number: 100,
    bigint: 100n,
    func: function (a, b, c) {},
    html: document.createElement("div")
});
```
will print...
```
object(Object) (7) {
    ["string"] => string(5) "hello"
    ["array"] => array(1) {
        [0] => string(6) "world!"
    }
    ["object"] => object(Object) (2) {
        ["subkey"] => array(3) {
            [0] => number(1)
            [1] => number(2)
            [2] => object(Object) (1) {
                ["deep"] => string(6) "nested"
            }
        }
        ["empty"] => object(Object) (0) {
        }
    }
    ["number"] => number(100)
    ["bigint"] => bigint(100)
    ["func"] => function {
        [name] => func
        [parameters] => array(3) {
            [0] => string(1) "a"
            [1] => string(1) "b"
            [2] => string(1) "c"
        }
    }
    ["html"] => HTMLElement(DIV)
}
```
