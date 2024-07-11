# Dependency injection
## Intro
Dependency injection refers a mechanism that initialize the an object in constructor with given parameters.

## Example
### Example 1
Take the example from Android Studio Docs. ([2] in Ref section)

A Car must have an engine.

The following code illustrates the use of dependency injection.

<p style="color:green">GOOD</p>

    class Car {
    
        private Engine engine;
    
        public void setEngine(Engine engine) {
            this.engine = engine;
        }
    
        public void start() {
            engine.start();
        }
    }
    
    class MyApp {
        public static void main(String[] args) {
            Car car = new Car();
            car.setEngine(new Engine());
            car.start();
        }
    }

The relationship of Car and Engine as follows.

![image](https://github.com/40843245/program_language/assets/75050655/530e9b59-cacc-4aea-bb9f-96695128db8d)


    class Car {
    
        private Engine engine = new Engine();
    
        public void start() {
            engine.start();
        }
    }
    
    
    class MyApp {
        public static void main(String[] args) {
            Car car = new Car();
            car.start();
        }
    }
## Pro
The pro of dependency injection:

1. Reusability of code
2. Ease of refactoring
3. Ease of testing

From the above example, image that you are a manufacturer of car. You may hope that the engine can be detached from the car since one can detach the engine when the engine is broken, one does NOT have to get a new car. The core concept can also apply to code. 

When one 
## Ref
[1] https://en.wikipedia.org/wiki/Dependency_injection

[2] https://developer.android.com/training/dependency-injection
