#                                                       Swift Programming Language

  Swift developed by under the leadership of Chris Lattner which be software engineer in the Aplle with Doug Gregor, John McCall, Ted Kremenek, Joe Groff and Aple Inc. Swift announced in  2 June 2014  at Apple Worldwide Developers Conferance .
While the Swift language was creating, many features from many other languages were taken. These languages are Objective-C, Rust, Haskell, Ruby, Python,  While the Swift language was creating, many features from many other languages were taken. These languages are Objective C, Rust, Haskell, Ruby, Python, C#, Clu, Dlang.  It was very much affected by Objective C.

 #                                                         Why was invented ?

  Objective C, is the main development language of IOS and MacOS systems. Objective C is a language that built on the C language by adding object-oriented features. We should know C language before start to learn Swift language. So the cost of learning Objective C is higher than the costs of learning other languages. Apple wanted to produce a new language which be modern and easy to learn to reduce this challenge. As a result Apple designed Swift programming langauge. 
  
  #                                                     When/why shall we use it ?
  
  ## When?
  Swift is a language that has been designed to develop products for Apple devices in general. So using Swift, it is possible to develop applications that can run smoothly on macOS, tvOS, iPadOS, watchOS and iOS devices.. But, there is an exception in this regard. Swift is an open source language, so it can work on other open source operating systems like Linux.  It is possible to develop an applications that can run on the Linux operating system using Swift.  But  Swift was originally designed to work on Apple products. That's why Swift is the programming language that can use the equipment of Apple products most efficiently.
If we want to develop an applications for Apple products, Swift is the best choice.

 ## Why shall we use it?
  1)	Swift to write and read is easier than many programming languages. When we compared to Objective-C, the number of codes that must be written to do the same operations is lesser than Objective C . So the product development process is faster. 

 ## Example  with Objective-C

if(myDelegate != nil){
  if([myDelegate respondsToSelector :
      @selector (scrollViewDidScroll:)]){
      [myDelegate scrollViewDidScroll:myScrollView];
      }
 }
 
 ## Example with Swift
 
 myDelegate?.scrollViewDidScroll?(myScrollView)
 
 
 2)	Swift is faster than other programming language in terms of performance.
 Swfit faster than Objective-C up to 2.6x and faster than Python 2.7 up to 8.4x .
 
 3)	Swift is a safe programming language. What does safe mean here? The reliability of a programming language is measured by how much it   can prevent code crashes and production errors. Swift’s development environment is Xcode and it has code editor, code debugger, test     environment like emulator and with other many features. So it prevents the occurrences of new errors.
 4)	ARC (Automatic Reference Counting) 
 Java and like C# languseges use garbage collector to delete unused class examples. Garbage collectors are very useful to increase      memory efficiency, but they can use up to twenty percent of processor power. 
Swift's Automatic Reference Counting feature detects automatically which samples are no longer used and deletes them. 
While doing this, it tire the device less because it does not use of the processor power.
 5)	Swift was also a very popular and loved language when it first came out. This shows that Swift will be used for many years and will maintain its place.


 6) Swift can be mount to Objective-C code seamlessly. At the same time, you can develop products using Swift together with Objective-C.
 
#                            How to setup an environment to use it in different platforms (windows, mac, linux)
 
 
 There is only one IDE that Apple can offer to us from the AppStore for free. Xcode A computer run on MacOS operating system is required to install Xcode.

  ## For macOS Operating Systems
  
We can develop applications for the following platforms with Xcode. MacOS iOS, watchOS, tvOS.

 ### How can i install Xcode on the macOS platform ?

It is the easiest way to use Xcode because this ide developed for apple products.
You can install Xcode from this link  https://apps.apple.com/tr/app/xcode/id497799835?mt=12 and accept all upload instructions

  ## For Windows Operating System 
  ### How can i use Xcode on Windows OS ?

It is possible to use Xcode on Windows, but there are some conditions. Our computer must have Intel processor. Xcode does not support AMD processors right now. And we need to install virtual machines to computer like VMware. You can install from this link https://www.vmware.com/products/workstation-pro/workstation-pro-evaluation.html
After that we should install macOS operating system to virtual machine. There are many macOS iso file to install on internet. You can follow this link. 
https://www.mediafire.com/folder/6p5rv8jd50cua/macOS_Catalina_10.15.3_by_Geekrar_(One_Full)
Finally we shoul install Xcode from this link https://apps.apple.com/tr/app/xcode/id497799835?mt=12

  ## For Linux Operating Systems
Swift installation on Ubuntu, now we need to install a component called Clang, which is the first and most important part of this installation.

Go to the Terminal and type:

sudo apt-get install clang

Since you need to install the Swift toolchain on Linux to a directory other than the system root, you will need to run the following command, using the actual path of your Swift installation:

export PATH=/path/to/Swift/usr/bin:”${PATH}”

Now it’s time to authenticate and very that you have the latest version of Swift by entering the swift command and passing the –version flag:

swift –version
Apple Swift version 2.2-dev (LLVM …, Clang …, Swift …)

The -dev suffix on the version number is used to indicate that it’s a development build, not a released version.

Now min level of the toolchain for XCode (the GCC compiler family, the gdb debugger, etc.) is the open-source and public to Unix and Linux platforms.

#                                       Example Codes for prime number calculations

func generatePrimes(to n: Int) -> [Int] {

    precondition(n > 5, "Input must be greater than 5")

    var arr : [Int] = Array<Int>(stride(from: 3, to: n, by: 2))     

    for index in 0... {
        let num : Int = arr.remove(at: index)
        arr = arr.filter{ $0 % num != 0 }
        arr.insert(num, at: index)
        if arr[index + 1] >= Int(floor(sqrtf(Float(n)))) { break }
    }

    arr.insert(2, at: 0)

    //Print Statements
    print("Prime numbers under \(n):")
    _ = arr.enumerated().map { (index, element) in print("\t\(index + 1). \(element)") }

    return arr
}



#                                           Things that are specific to this language?

Included some spesific features to Swift. 
```bash
Closures unified with function pointers.
Tuples and multiple return values.
Generics.
Fast and concise iteration over a range or collection.
Structs that support methods, extensions, and protocols.
Functional programming patterns, e.g., map and filter.
Powerful error handling built-in.
Advanced control flow with do, guard, defer, and repeat keywords.
Variables are always initialized before use.
Array indices are checked for out-of-bounds errors.
Integers are checked for overflow.
Optionals ensure that nil values are handled explicitly.
Memory is managed automatically.
Error handling allows controlled recovery from unexpected failures.
You don’t need a main() function. 
You also don’t need to write semicolons at the end of every statement.
```








