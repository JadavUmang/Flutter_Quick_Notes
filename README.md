# Flutter and Dart Notes
![Visitor Count](https://api.countapi.xyz/hit/jadavUmang.Flutter_Quick_Notes/visits?style=flat-square)

---

## Flutter

### Project Structure

1. **`.idea`**  
   - Stores project-related settings.

2. **`android`**  
   - Contains Android platform-specific resources, settings, and code.  
   - Used when Android-related changes are required.

3. **`build`**  
   - Used during testing mode to create executable files.  
   - Contains files for debugging and release (e.g., APK files).

4. **`ios`**  
   - Stores iOS platform-specific resources, settings, and code.  
   - Runnable `runnerXWorks` files and platform-specific changes are handled here.

5. **`lib`**  
   - The main library folder where all Dart/Flutter files are located.  
   - Entry point for a Flutter app is the `main.dart` file.

6. **`test`**  
   - Used for testing and improving user experience.  
   - Contains test-related files and code for writing test cases.

7. **`.gitignore`**  
   - Manages files excluded from version control (VCS).  
   - Ensures unnecessary files are not pushed to the repository.

8. **`.metadata`**  
   - Contains Flutter-related settings and metadata.

9. **`.packages`**  
   - Holds paths to all libraries/packages on the local machine.  
   - Includes:
     - Built-in packages: Predefined by Flutter.
     - User-defined packages: Created by the user.

10. **`pubspec.yaml`**  
    - Manages app-specific metadata and configurations.  
    - Used to add external dependencies (e.g., packages, assets, fonts, app versions).

11. **`pubspec.lock`**  
    - Helper file generated next to `pubspec.yaml`.  
    - Lists specific versions of each dependency to ensure consistency across development environments.

12. **`README.md`**  
    - Provides information about the project, its features, and usage instructions.  
    - Essential for Git repositories.

---

## Dart

### Overview

- Focuses on front-end user interfaces.  
- **Object-Oriented** and **Strongly Typed** (type must be known at compile time).  
- Combines features of Java, JavaScript, and C#.  
- Developed by Google in **2011**.  
- Known for fast development cycles, execution, and startup times.  
- Supports **asynchronous programming** using `async` and `await`.  
- Can be compiled both **Ahead of Time (AOT)** and **Just in Time (JIT)**.

> **JIT**: Reloads one page at a time.  
> **AOT**: Compiles the entire app when it's ready.

---

### Key Concepts

#### Printing

- `print()` - Prints output to the console.

#### Input and Output

- **Input**: `stdin.readLineSync()` reads user input from the console (in string format).  
- **Output**: `stdout.write()` writes output to the console.  
  - Example:  
    ```dart
    stdout.write('Your name is $name');
    ```

---

### Classes and Objects

- Similar to Java.  
- No need for the `new` keyword in newer versions.  

Example:  
```dart
class Demo {
  // Class definition
}

// Creating an object
Demo demoObject = Demo();
```

---

### Data Types

1. **Numbers**: `0-9`  
2. **Double**: Floating-point values  
3. **BigInt**: Large integer values  
4. **Character**: Alphanumeric data  
5. **String**: Array of characters  
6. **Boolean**: Logical `true` or `false` values  
   - Example: `bool a = true;`  
7. **Collections**:  
   - **List**: Stores multiple values in a single variable.  
   - **Map**: Key-value pairs.

---

### Variable Declaration

- By default, variables are `null`.  

Syntax:  
```dart
datatype variable_name;
```

Example:  
```dart
int a;       // Non-nullable variable
int? b;      // Nullable variable
```

---

### `var` vs `dynamic`

#### **`var`**
- Automatically assigns the type based on the initial value.  
- Type cannot be changed later.  

Example:  
```dart
var subject = "Maths";  // Type is set to String.
```

#### **`dynamic`**
- Type can be changed during runtime.  

Example:  
```dart
dynamic value;
value = "Hello";  // Type is String
value = 42;       // Type is Integer
```

---

### Notes on Dart Compilation

- **Dart Files**: Stored in the `lib` folder.  
- **JIT**: Reloads only a single page during development.  
- **AOT**: Compiles the whole app into a single `.dart` file for deployment.
