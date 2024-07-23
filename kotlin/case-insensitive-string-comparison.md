# Case-insensitive string comparison

In languages like Java and Scala, we use the method `equalsIgnoreCase` to compare two strings ignoring case considerations. 
We might assume that is the same case in Kotlin, but the equivalent to `equalsIgnoreCase` is the `equals` method with an optional parameter **ignoreCase** set to **true**:
```Kt
str1.equals(str2, ignoreCase = true)
```

_ref: https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.text/equals.html_
