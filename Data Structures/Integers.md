In Java, the `Integer` class is a wrapper class for the primitive `int` data type. It provides a range of methods for converting, comparing, and manipulating integer values. Below is a comprehensive list of methods available in the `Integer` class:

### 1. **Conversion Methods**
   - **`int intValue()`**: Converts the `Integer` object to a primitive `int`.
     ```java
     int num = integerObject.intValue();
     ```

   - **`long longValue()`**: Converts the `Integer` object to a primitive `long`.
     ```java
     long longNum = integerObject.longValue();
     ```

   - **`float floatValue()`**: Converts the `Integer` object to a primitive `float`.
     ```java
     float floatNum = integerObject.floatValue();
     ```

   - **`double doubleValue()`**: Converts the `Integer` object to a primitive `double`.
     ```java
     double doubleNum = integerObject.doubleValue();
     ```

   - **`byte byteValue()`**: Converts the `Integer` object to a primitive `byte`.
     ```java
     byte byteNum = integerObject.byteValue();
     ```

   - **`short shortValue()`**: Converts the `Integer` object to a primitive `short`.
     ```java
     short shortNum = integerObject.shortValue();
     ```

### 2. **Static Conversion Methods**
   - **`static String toString(int i)`**: Converts an `int` to a `String`.
     ```java
     String str = Integer.toString(123);
     ```

   - **`static String toString(int i, int radix)`**: Converts an `int` to a `String` in the specified radix (base).
     ```java
     String str = Integer.toString(123, 16); // Converts 123 to hexadecimal string "7b"
     ```

   - **`static int parseInt(String s)`**: Converts a `String` to an `int`.
     ```java
     int num = Integer.parseInt("123");
     ```

   - **`static int parseInt(String s, int radix)`**: Converts a `String` in the specified radix to an `int`.
     ```java
     int num = Integer.parseInt("7b", 16); // Converts hexadecimal string "7b" to 123
     ```

   - **`static Integer valueOf(String s)`**: Converts a `String` to an `Integer` object.
     ```java
     Integer integerObject = Integer.valueOf("123");
     ```

   - **`static Integer valueOf(String s, int radix)`**: Converts a `String` in the specified radix to an `Integer` object.
     ```java
     Integer integerObject = Integer.valueOf("7b", 16);
     ```

   - **`static Integer valueOf(int i)`**: Returns an `Integer` instance representing the specified `int`.
     ```java
     Integer integerObject = Integer.valueOf(123);
     ```

   - **`static String toBinaryString(int i)`**: Returns a string representation of the integer in binary (base 2).
     ```java
     String binaryStr = Integer.toBinaryString(123); // "1111011"
     ```

   - **`static String toHexString(int i)`**: Returns a string representation of the integer in hexadecimal (base 16).
     ```java
     String hexStr = Integer.toHexString(123); // "7b"
     ```

   - **`static String toOctalString(int i)`**: Returns a string representation of the integer in octal (base 8).
     ```java
     String octalStr = Integer.toOctalString(123); // "173"
     ```

### 3. **Comparison Methods**
   - **`int compareTo(Integer anotherInteger)`**: Compares two `Integer` objects.
     ```java
     int comparison = integerObject.compareTo(anotherInteger);
     ```

   - **`static int compare(int x, int y)`**: Compares two `int` values.
     ```java
     int comparison = Integer.compare(10, 20); // returns a negative value
     ```

   - **`static int compareUnsigned(int x, int y)`**: Compares two `int` values as unsigned.
     ```java
     int comparison = Integer.compareUnsigned(-10, 10);
     ```

### 4. **Bitwise Methods**
   - **`static int highestOneBit(int i)`**: Returns an `int` value with only the highest one bit set.
     ```java
     int highestBit = Integer.highestOneBit(10); // 8 (binary 1000)
     ```

   - **`static int lowestOneBit(int i)`**: Returns an `int` value with only the lowest one bit set.
     ```java
     int lowestBit = Integer.lowestOneBit(10); // 2 (binary 0010)
     ```

   - **`static int numberOfLeadingZeros(int i)`**: Returns the number of leading zeros in the binary representation.
     ```java
     int leadingZeros = Integer.numberOfLeadingZeros(10);
     ```

   - **`static int numberOfTrailingZeros(int i)`**: Returns the number of trailing zeros in the binary representation.
     ```java
     int trailingZeros = Integer.numberOfTrailingZeros(10);
     ```

   - **`static int bitCount(int i)`**: Returns the number of one-bits in the binary representation (Hamming weight).
     ```java
     int bitCount = Integer.bitCount(10); // 2 (binary 1010 has two 1's)
     ```

   - **`static int rotateLeft(int i, int distance)`**: Returns the value obtained by rotating the bits to the left.
     ```java
     int rotatedLeft = Integer.rotateLeft(10, 2); // Rotates bits of 1010 to left by 2 positions
     ```

   - **`static int rotateRight(int i, int distance)`**: Returns the value obtained by rotating the bits to the right.
     ```java
     int rotatedRight = Integer.rotateRight(10, 2);
     ```

   - **`static int reverse(int i)`**: Returns the value obtained by reversing the order of bits.
     ```java
     int reversed = Integer.reverse(10); // 10 -> 1010 (binary) reversed -> 0101 (binary)
     ```

   - **`static int reverseBytes(int i)`**: Returns the value obtained by reversing the order of the bytes.
     ```java
     int reversedBytes = Integer.reverseBytes(0x12345678);
     ```

   - **`static int signum(int i)`**: Returns the signum function of the argument (1 if positive, -1 if negative, 0 if zero).
     ```java
     int sign = Integer.signum(-10); // -1
     ```

### 5. **String Methods**
   - **`static int parseUnsignedInt(String s)`**: Parses the string argument as an unsigned decimal integer.
     ```java
     int unsignedNum = Integer.parseUnsignedInt("123");
     ```

   - **`static int parseUnsignedInt(String s, int radix)`**: Parses the string argument as an unsigned integer in the specified radix.
     ```java
     int unsignedNum = Integer.parseUnsignedInt("7b", 16); // 123
     ```

   - **`static String toUnsignedString(int i)`**: Returns a string representation of the integer as an unsigned decimal value.
     ```java
     String unsignedStr = Integer.toUnsignedString(-123);
     ```

   - **`static String toUnsignedString(int i, int radix)`**: Returns a string representation of the integer as an unsigned value in the specified radix.
     ```java
     String unsignedStr = Integer.toUnsignedString(-123, 16);
     ```

### 6. **Constants**
   - **`static final int MIN_VALUE`**: The minimum value an `int` can have (`-2^31`).
     ```java
     int minValue = Integer.MIN_VALUE;
     ```

   - **`static final int MAX_VALUE`**: The maximum value an `int` can have (`2^31-1`).
     ```java
     int maxValue = Integer.MAX_VALUE;
     ```

   - **`static final Class<Integer> TYPE`**: The `Class` instance representing the `int` type.
     ```java
     Class<Integer> type = Integer.TYPE;
     ```

   - **`static final int SIZE`**: The number of bits used to represent an `int` value in binary (32).
     ```java
     int size = Integer.SIZE;
     ```

   - **`static final int BYTES`**: The number of bytes used to represent an `int` value (4).
     ```java
     int bytes = Integer.BYTES;
     ```

### 7. **Miscellaneous Methods**
   - **`static Integer decode(String nm)`**: Decodes a `String` into an `Integer`.
     ```java
     Integer decoded = Integer.decode("0x7b"); // 123
     ```

   - **`static int hashCode(int value)`**: Returns a hash code for an `int` value.
     ```java
     int hashCode = Integer.hashCode(123);
     ```

   - **`static int sum(int a, int b)`**: Returns the sum of two integers.
     ```java
     int sum = Integer.sum(10, 20); // 30
     ```

   - **`static int max(int a, int b)`**: Returns the greater of two integers.
     ```java
     int max = Integer.max(10, 20); // 20
     ```

   - **`static int min(int a, int b)`**: Returns the smaller of two integers.
     ```java
     int min = Integer.min(10, 20); // 10
     ```

This list covers the essential methods available for the `Integer` class in Java. These methods provide a wide range of functionalities for handling and manipulating integer values in your programs.