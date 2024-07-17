# backing field
## Intro
property with backing field can override the declaration the behavoir when accessing the value of property. 

In C#, a famous setter-getter property is a kind of property with backing field.

## Example
### In C#
    
    private int m_Capacity;
    public int Capacity
    {
        get { return m_Capacity > 0 ? m_Capacity : -666; }
        set { m_Capacity = value; }
    }

### In Kotlin
    
    var counter = 0 // the initializer assigns the backing field directly
        set(value) {
            if (value >= 0)
                field = value
                // counter = value // ERROR StackOverflow: Using actual name 'counter' would make setter recursive
        }

## Ref

Backing fields in C#.

https://stackoverflow.com/questions/3272889/properties-backing-field-what-is-it-good-for

Backing fields in Kotlin.

https://kotlinlang.org/docs/properties.html#backing-fields
https://kotlinlang.org/docs/properties.html#backing-fields
