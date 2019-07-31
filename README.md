## SwiftUI Grid

SwiftUI Grid view layout with auto-sizing items and flexible column count.

<center>
<img src="Resources/preview.png"/>
</center>

## Examples

```swift
/// Simple grid.

Grid(0...100) {
    Text("\($0)")
}
```

```swift
/// Grid with minimum item width and fixed item height.

Grid(self.planets, minimumItemWidth: 320, spacing: 16) {
    PlanetView(planet: $0)
        .frame(height: 400)
        .onTapGesture {
            print("Selection:", $0)
        }
}
.edgesIgnoringSafeArea(.all)
```

## Requirements

- Swift 5+
- iOS 13+
- macOS 10.15+

## Roadmap
- ZStack based grid instead of 'VStack of HStacks'
- Support for watchOS
- Items selection and rearranging
- UITests
- 'CSS Grid'-like features

## Contibutions
Feel free to contribute via fork/pull request to master branch. If you want to request a feature or report a bug please start a new issue.
