# SwiftUI Cheatsheet

SwiftUI is a declarative framework for building user interfaces in Swift. Here is an overview of some of its basic syntax and features.

## Views

### Text
```
Text("Hello, world!")
    .font(.title)
    .foregroundColor(.blue)
```

### Image
```
Image("imageName")
    .resizable()
    .aspectRatio(contentMode: .fit)
```

### Button
```
Button(action: {
    // Button action
}) {
    Text("Button")
}
```

### List
```
List {
    Text("Item 1")
    Text("Item 2")
}
```

## Layout

### VStack
```
VStack {
    Text("Top")
    Text("Middle")
    Text("Bottom")
}
```

### HStack
```
HStack {
    Text("Left")
    Text("Center")
    Text("Right")
}
```

### ZStack
```
ZStack {
    Image("backgroundImage")
        .resizable()
        .aspectRatio(contentMode: .fill)
    Text("Foreground")
}
```

## Navigation

### NavigationView
```
NavigationView {
    List {
        NavigationLink(destination: DetailView()) {
            Text("Item 1")
        }
        NavigationLink(destination: DetailView()) {
            Text("Item 2")
        }
    }
}
```

### Presentation
```
struct ContentView: View {
    @State var showModal = false

    var body: some View {
        Button(action: {
            showModal = true
        }) {
            Text("Show Modal")
        }
        .sheet(isPresented: $showModal) {
            ModalView()
        }
    }
}
```

## Resources

- [SwiftUI Documentation](https://developer.apple.com/documentation/swiftui)
- [SwiftUI Tutorials](https://www.hackingwithswift.com/quick-start/swiftui)