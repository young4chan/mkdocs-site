An example for a codeblock for Python:

```py title="mathematics.py" linenums="1"
def add(x, y):
    return x + y

def subtract(x, y):
    return x - y

def multiply(x, y):
    return x * y

def divide(x, y):
    if y == 0:
        return "Error: Division by zero is not allowed."
    else:
        return x / y

def main():
    print("Basic Calculator")
    print("1. Addition")
    print("2. Subtraction")
    print("3. Multiplication")
    print("4. Division")
    
    choice = input("Enter your choice (1/2/3/4): ")
    
    if choice in ('1', '2', '3', '4'):
        num1 = float(input("Enter first number: "))
        num2 = float(input("Enter second number: "))
        
        if choice == '1':
            print(num1, "+", num2, "=", add(num1, num2))
        elif choice == '2':
            print(num1, "-", num2, "=", subtract(num1, num2))
        elif choice == '3':
            print(num1, "*", num2, "=", multiply(num1, num2))
        elif choice == '4':
            print(num1, "/", num2, "=", divide(num1, num2))
    else:
        print("Invalid input")

if __name__ == "__main__":
    main()

```

``` js title="mathematics.js" linenums='1' hl_lines="9-11"
function add(x, y) {
    return x + y;
}

function subtract(x, y) {
    return x - y;
}

function multiply(x, y) {
    return x * y;
}

function divide(x, y) {
    if (y === 0) {
        return "Error: Division by zero is not allowed.";
    } else {
        return x / y;
    }
}

function main() {
    console.log("Basic Calculator");
    console.log("1. Addition");
    console.log("2. Subtraction");
    console.log("3. Multiplication");
    console.log("4. Division");
    
    // For simplicity, this example uses hardcoded inputs.
    // In a real application, you would use a method to get user input.
    let choice = prompt("Enter your choice (1/2/3/4): ");
    
    if (choice === '1' || choice === '2' || choice === '3' || choice === '4') {
        let num1 = parseFloat(prompt("Enter first number: "));
        let num2 = parseFloat(prompt("Enter second number: "));
        
        if (choice === '1') {
            console.log(`${num1} + ${num2} = ${add(num1, num2)}`);
        } else if (choice === '2') {
            console.log(`${num1} - ${num2} = ${subtract(num1, num2)}`);
        } else if (choice === '3') {
            console.log(`${num1} * ${num2} = ${multiply(num1, num2)}`);
        } else if (choice === '4') {
            console.log(`${num1} / ${num2} = ${divide(num1, num2)}`);
        }
    } else {
        console.log("Invalid input");
    }
}

main();
```