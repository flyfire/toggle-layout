# Android Toggle Layout

[![Release](https://jitpack.io/v/philip-bui/toggle-layout.svg)](https://jitpack.io/#philip-bui/toggle-layout)
[![Downloads](https://jitpack.io/v/philip-bui/toggle-layout/month.svg)](https://jitpack.io/#philip-bui/toggle-layout)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/philip-bui/toggle-layout/blob/master/LICENSE)

An extension of LinearLayout that allows users to expand and collapse views using fade down and fade up animations. 

- Configurable. Minimum children to show while collapsed.
- Saved State. State is preserved upon screen rotation or recreation.
- Animated - Transitions to expanded and collapsed states.
- Thread safety - Expand and collapse animations do not interrupt, override or queue after each other. Users only trigger transitions after state has been completed.

## Requirements

- Android SDK 1.0+.

## Installation

```gradle
repositories {
     jcenter()
     maven { url "https://jitpack.io" }
}
dependencies {
     implementation 'com.github.philip-bui:toggle-layout:1.0.0'
}
```

## Usage

```xml
<com.nextgeneration.ToggleLayout
	...
	app:minChildren="1">

</com.nextgeneration.ToggleLayout>
```

```java
ToggleLayout toggleLayout = null;
toggleLayout.expand(); // Expands or maintains expanded state.
toggleLayout.collapse(); // Collapses or maintains collapsed state.
toggleLayout.toggle(); // Expands or collapses depending on state.
```

# License

ToggleLayout is available under the MIT license. [See LICENSE](https://github.com/philip-bui/toggle-layout/blob/master/LICENSE) for details.

