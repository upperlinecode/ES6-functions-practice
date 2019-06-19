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

4. Some older databases can't handle special characters like spaces, @, #, $, etc. Create a function called `checkSpecialCharacters` that checks to see if a string contains any of the following special characters: ` ` (a space), `!`, `@`, `#`, or `$`. If the string contains one of those characters, it should return `true`. If the string doesn't contain one of those characters, it should return `false`.

Example:

```js
checkSpecialCharacters("batman and robin") // Returns True
checkSpecialCharacters("jokerAndPenguin") // Returns False

```

5. On the other hand, newer sites **require** that users include one or more special characters in their passwords. Create a function called `requireSpecialCharacters` that checks to see if a string contains _two or more_ of the following special characters: ` ` (a space), `!`, `@`, `#`, `$`, `%`, `^`, `&`, `-`, `_`, or `*`. If the string contains two or more of those characters, it should return `true`. If the string contains one or fewer of those characters, it should return `false`.

Example:

```js
requireSpecialCharacters("mighty-Morphin_p0wer Rangers!") // Returns True
requireSpecialCharacters("hereWeG0!") // Returns False
requireSpecialCharacters("ohnoanotherbadguy") // Returns False

```

### Spicy

6. Newer sites also require that passwords contain a combination of the following: uppercase letters, lowercase letters, numbers, and special characters (see #5). Create a function called `checkMultipleSymbols` that checks to see if a string contains one of each of these types of characters.

Example:

```js
checkMultipleSymbols("This1sMyBestP@ssw0rd") // Returns True
checkMultipleSymbols("NotGoodEnough!") // Returns False
checkMultipleSymbols("eventhoughthisisareallylongpassworditstillisntgoodenough") // Returns False

```

7. Update your `checkMultipleSymbols` function to return a message to the user indicating which type of character is missing from their proposed password. If the password contains all four types of characters, then return "Great password!"

Example:

```js
checkMultipleSymbols("This1sMyBestP@ssw0rd") // Returns "Great password"
checkMultipleSymbols("NotGoodEnough!") // Returns "Missing a special character"
checkMultipleSymbols("eventhoughthisisareallylongpassworditstillisntgoodenough") // Returns "Missing a capital letter, a number, and a special character"

```

8. Update your `checkMultipleSymbols` function again to provide a user with some visual feedback about the strength of their password. This could be in the form of a color-coded message or progress bar or something of your own design.

For example, if the password contains all four types of characters, then it could return "Great password!" on a green background. If it's missing one type of character, maybe the message is on a yellow background; if it's missing two, it could be on an orange background; and if it's missing three, it could be on a red background.

Use your creativity to help the user generate a secure password!

