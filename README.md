# number_to_persian_word

A Library that Makes You Able to Convert any Number to Persian Word.
This Library Supports Decimal Point, Negative Numbers and Percent.

### `NumberToPersianWord.js`

Main Library File is `./dist/NumberToPersianWord.js`. Copy it in Your Project, then Add It into Your HTML File. Enjoy :)

### `With npm`

use `npm i number_to_persian_word` or `yarn add number_to_persian_word`
then use:

```javascript
const NumberToPersianWord = require("number_to_persian_word");
```

or you can use:

```javascript
import NumberToPersianWord from "number_to_persian_word";
```

### `Functions`

To Use This Library You Can Call All of it's Functions using **NumberToPersianWord.functionName();**

#### `NumberToPersianWord.convert(number);`

Input: a number as int or float or string

Output: Converted Number to it's Word (string)

Example:

```javascript
NumberToPersianWord.convert(123); // صد و بیست و سه
NumberToPersianWord.convert(-123.2); // منفی صد و بیست و سه ممیز دو دهم
NumberToPersianWord.convert("-123.26%"); //منفی صد و بیست و سه ممیز بیست و شش صدم درصد
```

#### `NumberToPersianWord.sliceNumber(number,separator=",");`

Input: a number as int or float or string and a separator(Optional) (number should be in english)

Output: The number is separated by three digits of the three digits, then return it. (string)

Example:

```javascript
NumberToPersianWord.sliceNumber(12345); // 12,345
```

#### `NumberToPersianWord.convertEnToPe(number);`

Input: a number as int or float or string (English Digits)

Output: Returns Converted English Digits into Persian Digits. (string)

Example:

```javascript
NumberToPersianWord.convertEnToPe(123); // ۱۲۳
```

#### `NumberToPersianWord.convertPeToEn(number);`

Input: a number as string (Persian Digits)

Output: Returns Converted Persian Digits into English Digits. (string)

Example:

```javascript
NumberToPersianWord.convertPeToEn("۱۲۳"); // 123
```

`For More Examples See index.js`
