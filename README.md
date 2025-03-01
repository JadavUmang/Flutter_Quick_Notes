# Important

## Flutter

### Project Structure

1. **.idea/**  
   - Stores project-related settings.

2. **android/**  
   - Android platform-specific resources, settings & code.
   - Used when Android-related changes are required.

3. **build/**  
   - Testing mode - code is created in an executable file.
   - Used for debugging purposes when running the app.
   - Contains all release-related files like APK.

4. **ios/**  
   - Platform-specific resources, settings & code for iOS.
   - iOS/platform-related changes can be made here.
   - The runnable `Runner.xcworkspace` file is stored here.

5. **lib/**  
   - Library folder containing all Dart/Flutter-related files.
   - Main folder with maximum usage.
   - Entry point for a Flutter app (`main.dart` file).

6. **test/**  
   - Used to improve user experience or test user experience.
   - Contains test-related files.
   - If test cases are written, they will be added here.

7. **.gitignore**  
   - Used in Version Control System (VCS).
   - Removes unnecessary files.
   - Operations like push, pop, pull, etc., can be performed.
   - Specifies files that should not be pushed.

8. **.metadata**  
   - Contains data related to Flutter.
   - Manages all Flutter-related settings and data.

9. **.packages**  
   - Stores package paths.
   - Two types of packages:
     - Built-in packages: Predefined by Flutter.
     - User-defined packages: Created by the user.

10. **pubspec.yaml**  
    - Contains Flutter app metadata and configurations.
    - Specifies dependencies such as external packages, image assets, font files, app version, etc.
    - Changes in this file allow adding external dependencies.

11. **pubspec.lock**  
    - Dependent on `pubspec.yaml` file.
    - Creates log files.
    - Lists the specific versions of each dependency used in the app.
    - Ensures consistency across different developer machines.

12. **README.md**  
    - Used when creating a Git repository.
    - Contains information about the project, its usage, and specifications.

---

## Dart

- Focuses on frontend user interface.
- Object-Oriented and strongly typed (variable type must be known at compile time).
- Combination of Java, JavaScript, and C#.
- Developed by Google in 2011.
- Extremely fast development cycles, fast execution, and startup times.
- Uses `async` and `await` for asynchronous programming.
- Supports both Ahead-of-Time (AOT) and Just-in-Time (JIT) compilation.

### Compilation Modes
- **JIT (Just-in-Time):** Reloads only one page.
- **AOT (Ahead-of-Time):** The whole app is compiled into a single `.dart` file before deployment.
- Dart files are stored under the `lib/` folder.

### Print Statements
```dart
print("Hello, World!"); // Prints output to console
```

### Standard Input & Output
```dart
stdin.readLineSync(); // Reads user input as a string
stdout.write("Enter your name: ");
```

### Class & Object
```dart
class Demo {}
Demo obj = Demo(); // Creating an object (no 'new' keyword required)
```

### Data Types
- `int` - Whole numbers (0-9)
- `double` - Floating-point values
- `bigint` - Large integer numbers
- `String` - Alphanumeric data
- `bool` - Boolean values (`true` or `false`)
- **Collections**:
  - `List` (Similar to arrays)
  - `Map` (Key-value pairs)

### Variable Declaration
```dart
int a;      // Non-nullable variable
int? b;     // Nullable variable
```

### `var` vs `dynamic`
```dart
var subject = "Maths"; // Type is inferred and cannot change

dynamic variable;
variable = "Hello";  // String
variable = 42;       // Integer
```

### Functions
```dart
void printName() {
  print("Your name");
}
```

---

## Flutter

### Widgets in Flutter
All UI components in Flutter are widgets.

#### **Text Widget**
```dart
Text(
  'Hello, welcome to my app',
  style: TextStyle(
    fontSize: 25,
    color: Colors.white,
    fontWeight: FontWeight.bold,
  ),
)
```

#### **Button Widgets**
```dart
ElevatedButton(
  onPressed: () {
    print('Button Clicked');
  },
  child: Text('Click Me'),
)
```

#### **Adding an Image**
To add an image, store it in `assets/images/` and update `pubspec.yaml`:
```yaml
flutter:
  assets:
    - assets/images/
```
Load the image in Flutter:
```dart
Image.asset('assets/images/logo.png')
```

---

## 🎯 Conclusion
This README provides an overview of the Flutter project structure, Dart programming concepts, and Flutter UI components. Happy coding! 🚀
