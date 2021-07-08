# iOSHowTos

## Table of contents

[#1 How to change color of navigation bar in SwiftUI?](https://github.com/bnulo/ioshowtos#1-how-to-change-color-of-navigation-bar-in-swiftui)

## #1 How to change color of navigation bar in SwiftUI?

#### Solution #1
```swift
// BEFORE:

import SwiftUI

struct ContentView: View {
    var body: some View {
        NavigationView {
              List {
                ForEach(0..<12, id: \.self, content: { i in
                  NavigationLink("List Item \(i)", destination: Text("\(i)"))
                })
              }
              .navigationBarTitle("Title")
            }
    }
}

// AFTER:

import SwiftUI
// 1- add
import UIKit

struct ContentView: View {
    var body: some View {
        NavigationView {
              List {
                ForEach(0..<12, id: \.self, content: { i in
                  NavigationLink("List Item \(i)", destination: Text("\(i)"))
                })
              }
              .navigationBarTitle("Title")
            }
        // 4- add
        .navigationBarColor(backgroundColor: .black, tintColor: .systemPink)
    }
}

// 2- add
struct NavigationBarColor: ViewModifier {

    init(backgroundColor: UIColor, tintColor: UIColor) {
        let coloredAppearance = UINavigationBarAppearance()
        coloredAppearance.configureWithOpaqueBackground()
        coloredAppearance.backgroundColor = backgroundColor
        coloredAppearance.titleTextAttributes = [.foregroundColor: tintColor]
        coloredAppearance.largeTitleTextAttributes = [.foregroundColor: tintColor]

        UINavigationBar.appearance().standardAppearance = coloredAppearance
        UINavigationBar.appearance().scrollEdgeAppearance = coloredAppearance
        UINavigationBar.appearance().compactAppearance = coloredAppearance
        UINavigationBar.appearance().tintColor = tintColor
    }

    func body(content: Content) -> some View {
        content
    }
}

// 3- add
extension View {
  func navigationBarColor(backgroundColor: UIColor, tintColor: UIColor) -> some View {
    self.modifier(NavigationBarColor(backgroundColor: backgroundColor, tintColor: tintColor))
  }
}

```

#### Solution #2
```swift
import SwiftUI

@main
struct SwiftVideosApp: App {
    init() {
        let backgroundColor = UIColor.black
        let tintColor = UIColor.systemPink
        let coloredAppearance = UINavigationBarAppearance()
        coloredAppearance.configureWithOpaqueBackground()
        coloredAppearance.backgroundColor = backgroundColor
        coloredAppearance.titleTextAttributes = [.foregroundColor: tintColor]
        coloredAppearance.largeTitleTextAttributes = [.foregroundColor: tintColor]

        UINavigationBar.appearance().standardAppearance = coloredAppearance
        UINavigationBar.appearance().scrollEdgeAppearance = coloredAppearance
        UINavigationBar.appearance().compactAppearance = coloredAppearance
        UINavigationBar.appearance().tintColor = tintColor
    }
    var body: some Scene {
        WindowGroup {
            ContentView()
        }
    }
}

```

