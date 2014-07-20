OptionalBug
===========

I have a class so defined:

class User {

    var name : String?
}
I use it in my ViewController using the code:

import UIKit

class ViewController: UIViewController {

    let user : User = User()
}
I have the compilation error

User is not constructible with ()

I know that the properties in Swift must have a default, but the optional has one (nil). The error disappear if I initialize the property "name" to nil or add an init() initializer. But I don't understand why my optional has not nil by default.

By the way, the following code in playground compiles perfectly:

class ViewController: UIViewController {

    let user : User = User()
}

class User {

    var name : String?
}
let vc = ViewController()
And it is strange.


EDIT: The error happens only if the User class is defined in a separated file. XCode is Beta 3