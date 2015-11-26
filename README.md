This is a very simple fork of [Mocha](https://github.com/mochajs/mocha).

The main difference that this fork brings is to reset the require cache before
requiring each test file. This lets you not worry about requires in different
test files stomping over each other.

Todo: reset the global before running each test file, this way each test file
will be truly isolated outside of modifying "this".
