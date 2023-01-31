# Class-name-binding-

class Foo {
 // Foo inside this block is a const binding
}
// Foo here is a let binding
For example,
class A {
 foo() {
 A = null; // will throw at runtime as A inside the class is a `const` binding
 }
}
A = null; // will NOT throw as A here is a `let` binding
