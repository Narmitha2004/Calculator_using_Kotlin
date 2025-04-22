# Calculator_using_Kotlin
fun main() {
//     println("Enter the number1 and number2 to calculate") 
    val num1=10
    val num2=9

    // Check if inputs are valid
    
    println("*************Ready to play**************")
    println("1. Addition")
    println("2. Subtraction")
    println("3. Multiplication")
    println("4. Division")
    
    val operation = 1
println("Your Operation is $operation")
    when (operation) {
        1 -> add(num1, num2)
        2 -> sub(num1, num2)
        3 -> mul(num1, num2)
        4 -> {
            if (num2 == 0) {
                println("Cannot divide by zero.")
            } else {
                div(num1, num2)
            }
        }
        else -> println("Invalid choice. Please select a number between 1 and 4.")
    }
}

fun add(a: Int, b: Int) {
    println("Your addition is ${a + b}")
}

fun sub(a: Int, b: Int) {
    println("Your subtraction is ${a - b}")
}

fun mul(a: Int, b: Int) {
    println("Your multiplication is ${a * b}")
}

fun div(a: Int, b: Int) {
    println("Your division is ${a / b}")
}
