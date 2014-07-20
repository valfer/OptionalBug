OptionalBug
===========

Project to demonstrate (possible) bug of Swift beta 3

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

The error happens only if the User class and ViewController class are defined in separated files. XCode is Beta 3