The `Double` class in Java is a wrapper class for the primitive `double` data type. It provides various methods for converting, comparing, and manipulating double-precision floating-point values. Below is a comprehensive list of methods available in the `Double` class:

### 1. **Conversion Methods**
   - **`double doubleValue()`**: Converts the `Double` object to a primitive `double`.
     ```java
     double num = doubleObject.doubleValue();
     ```

   - **`int intValue()`**: Converts the `Double` object to a primitive `int`, truncating the decimal part.
     ```java
     int intNum = doubleObject.intValue();
     ```

   - **`long longValue()`**: Converts the `Double` object to a primitive `long`, truncating the decimal part.
     ```java
     long longNum = doubleObject.longValue();
     ```

   - **`float floatValue()`**: Converts the `Double` object to a primitive `float`.
     ```java
     float floatNum = doubleObject.floatValue();
     ```

   - **`byte byteValue()`**: Converts the `Double` object to a primitive `byte`, truncating the decimal part.
     ```java
     byte byteNum = doubleObject.byteValue();
     ```

   - **`short shortValue()`**: Converts the `Double` object to a primitive `short`, truncating the decimal part.
     ```java
     short shortNum = doubleObject.shortValue();
     ```

### 2. **Static Conversion Methods**
   - **`static String toString(double d)`**: Converts a `double` to a `String`.
     ```java
     String str = Double.toString(123.45);
     ```

   - **`static double parseDouble(String s)`**: Converts a `String` to a `double`.
     ```java
     double num = Double.parseDouble("123.45");
     ```

   - **`static Double valueOf(String s)`**: Converts a `String` to a `Double` object.
     ```java
     Double doubleObject = Double.valueOf("123.45");
     ```

   - **`static Double valueOf(double d)`**: Returns a `Double` instance representing the specified `double` value.
     ```java
     Double doubleObject = Double.valueOf(123.45);
     ```

   - **`static long doubleToLongBits(double value)`**: Converts a `double` to its corresponding bit representation as a `long`.
     ```java
     long bits = Double.doubleToLongBits(123.45);
     ```

   - **`static long doubleToRawLongBits(double value)`**: Converts a `double` to its raw bit representation as a `long`, without collapsing NaN values.
     ```java
     long rawBits = Double.doubleToRawLongBits(123.45);
     ```

   - **`static double longBitsToDouble(long bits)`**: Converts a `long` bit representation back to a `double`.
     ```java
     double num = Double.longBitsToDouble(bits);
     ```

   - **`static double sum(double a, double b)`**: Returns the sum of two `double` values.
     ```java
     double sum = Double.sum(123.45, 67.89);
     ```

   - **`static double max(double a, double b)`**: Returns the greater of two `double` values.
     ```java
     double max = Double.max(123.45, 67.89);
     ```

   - **`static double min(double a, double b)`**: Returns the smaller of two `double` values.
     ```java
     double min = Double.min(123.45, 67.89);
     ```

### 3. **Comparison Methods**
   - **`int compareTo(Double anotherDouble)`**: Compares two `Double` objects.
     ```java
     int comparison = doubleObject.compareTo(anotherDouble);
     ```

   - **`static int compare(double d1, double d2)`**: Compares two `double` values.
     ```java
     int comparison = Double.compare(123.45, 67.89); // returns a positive value
     ```

   - **`static boolean isNaN(double v)`**: Checks if the specified `double` value is `NaN` (Not-a-Number).
     ```java
     boolean isNaN = Double.isNaN(0.0 / 0.0);
     ```

   - **`boolean isNaN()`**: Checks if the `Double` object is `NaN`.
     ```java
     boolean isNaN = doubleObject.isNaN();
     ```

   - **`static boolean isInfinite(double v)`**: Checks if the specified `double` value is positive or negative infinity.
     ```java
     boolean isInfinite = Double.isInfinite(1.0 / 0.0);
     ```

   - **`boolean isInfinite()`**: Checks if the `Double` object is positive or negative infinity.
     ```java
     boolean isInfinite = doubleObject.isInfinite();
     ```

### 4. **String Methods**
   - **`static String toHexString(double d)`**: Returns a hexadecimal string representation of the `double` value.
     ```java
     String hexStr = Double.toHexString(123.45);
     ```

   - **`static String toString(double d)`**: Returns a `String` representation of the `double` value.
     ```java
     String str = Double.toString(123.45);
     ```

   - **`static Double valueOf(double d)`**: Returns a `Double` object holding the `double` value.
     ```java
     Double doubleObject = Double.valueOf(123.45);
     ```

   - **`static Double valueOf(String s)`**: Returns a `Double` object holding the value represented by the string.
     ```java
     Double doubleObject = Double.valueOf("123.45");
     ```

### 5. **Constants**
   - **`static final double MIN_VALUE`**: The smallest positive `double` value (`2^-1074`).
     ```java
     double minValue = Double.MIN_VALUE;
     ```

   - **`static final double MAX_VALUE`**: The largest positive `double` value (`2^1023`).
     ```java
     double maxValue = Double.MAX_VALUE;
     ```

   - **`static final double MIN_NORMAL`**: The smallest positive normalized `double` value (`2^-1022`).
     ```java
     double minNormal = Double.MIN_NORMAL;
     ```

   - **`static final double NaN`**: A constant holding a Not-a-Number (NaN) value of type `double`.
     ```java
     double nanValue = Double.NaN;
     ```

   - **`static final double POSITIVE_INFINITY`**: A constant holding the positive infinity of type `double`.
     ```java
     double posInf = Double.POSITIVE_INFINITY;
     ```

   - **`static final double NEGATIVE_INFINITY`**: A constant holding the negative infinity of type `double`.
     ```java
     double negInf = Double.NEGATIVE_INFINITY;
     ```

   - **`static final int SIZE`**: The number of bits used to represent a `double` value in binary (64).
     ```java
     int size = Double.SIZE;
     ```

   - **`static final int BYTES`**: The number of bytes used to represent a `double` value (8).
     ```java
     int bytes = Double.BYTES;
     ```

   - **`static final Class<Double> TYPE`**: The `Class` instance representing the `double` type.
     ```java
     Class<Double> type = Double.TYPE;
     ```

### 6. **Miscellaneous Methods**
   - **`static Double decode(String nm)`**: Decodes a `String` into a `Double`.
     ```java
     Double decoded = Double.decode("123.45");
     ```

   - **`static int hashCode(double value)`**: Returns a hash code for a `double` value.
     ```java
     int hashCode = Double.hashCode(123.45);
     ```

   - **`static double sum(double a, double b)`**: Returns the sum of two `double` values.
     ```java
     double sum = Double.sum(123.45, 67.89);
     ```

   - **`static double max(double a, double b)`**: Returns the greater of two `double` values.
     ```java
     double max = Double.max(123.45, 67.89);
     ```

   - **`static double min(double a, double b)`**: Returns the smaller of two `double` values.
     ```java
     double min = Double.min(123.45, 67.89);
     ```

This list covers the essential methods available for the `Double` class in Java. These methods provide a wide range of functionalities for handling and manipulating double-precision floating-point values in your programs.