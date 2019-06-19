# ES6-functions-practice

## Password Madness!

Have you ever gone to a website and had that frustrating experience where the password expectations are crazy? In this lab, you'll be working on building password generators and verifiers, using ES6 Functions syntax.

Remember that function syntax in ES6 looks like this:

```js
//defining a function
const myFunc = (name) => {
  return "hello " + name
}

// calling a function
myFunc("Taylor") // Returns "hello Taylor"
```

### Mild
 1. Create a function called `basicPasswordCheck()` that takes in a password string and returns "This is a valid password" if the password has 10 or more characters, and "This password is too short" if the password has less than 10 characters.

Example:

```js
basicPasswordCheck("hello") // Returns "This password is too short"
basicPasswordCheck("thisisalongpassword") // Returns "This is a valid password"

```

 2. Create a function called `basicPasswordGenerator()` that takes a number and creates a new string that is the length of the input number. The string can be anything at all, as long as it is the right length. There are lots of ways to do this!

Example:

 ```js
 basicPasswordGenerator(10) // Returns "aaaaaaaaaa" or "1234567890" or "ab4jo012d4" or any other 10 character string.
 basicPasswordGenerator(3) // Returns "rts" or "111" or any other 3 character string.

 ```

 3. Create a function called `confirmSamePasswords` that checks to make sure that two inputted strings are the same. If the two strings are the same, it should return `true`. If the two strings are different, it should return `false`.

 Example:

 ```js
 confirmSamePasswords("donut2AreDeliciou3!", "donut2AreDeliciou3!") // Returns True
 confirmSamePasswords("Dogs&CatsRGr8", "IlikePeanutButter") // Returns False

 ```

### Medium



### Spicy
