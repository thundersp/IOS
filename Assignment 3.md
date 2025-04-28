## Basic FlashLight App

### Steps Below
1. Open Xcode and create a new IOS App
2. Name the project "FlashLight"
3. In Main, inside Safe area, add Label and Button from the Library, from the plus icon in the right top
4. Rename the label as "FlashLight"
5. Open the ViewController.swift file and Main in split screen, hold option and click on the ViewController.swift file to open it in a split view.
6. Hold control and click on Button, drag the blue line to ViewController in split view, and release, it will give options, choose "Action" for Connection, "onOFF' for Name, "UIButton" for Type.
7. It will form a function in ViewController.swift file, which will be called when the button is pressed. in that code, write the following code:
    ```swift
    @IBAction func onOFF(_ sender: UIButton) {
    isLightOn = !isLightOn
            print("On off is now \(isLightOn)")
            if isLightOn {
                view.backgroundColor = .white
            }
            else {
                view.backgroundColor = .black
            }
    }
    ```
8. The final ViewController will look like this:
    ```swift
    import UIKit

    class ViewController: UIViewController {

        var isLightOn = false

        override func viewDidLoad() {
            super.viewDidLoad()
        }

        @IBAction func onOFF(_ sender: UIButton) {
            isLightOn = !isLightOn
            print("On off is now \(isLightOn)")
            if isLightOn {
                view.backgroundColor = .white
            }
            else {
                view.backgroundColor = .black
            }
        }
    }
    ```
    
9. Done