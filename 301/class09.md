Functional Programming
1. What is functional programming?
    - [Definition](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)
    >Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data — Wikipedia
2. What is a pure function and how do we know if something is a pure function?
    - it ouputs the same thing every time with the same input and it doesn't have any side effects.
3. What are the benefits of a pure function?
    - it's easier to test
4. What is immutability?
    - unchanign over time. in this context it means data not changing.
5. What is Referential transparency?
    - the combination of pure and immutable functions.
Node.js
1. What is a module?
    - different files that we split of our code into common groups.
2. What does the word ‘require’ do?
    - import essentially.
3. How do we bring another module into the file the we are working in?
    - using require and passing in the path
4. What do we have to do to make a module available?
    - module.export