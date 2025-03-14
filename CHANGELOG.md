Date format: DD/MM/YYYY

## Unreleased

- New FluentIcons gallery showcase in example project https://github.com/bdlukaa/fluent_ui/issues/123
- Updated FluentIcons as per 30/12/2021
- Renamed `FluentIcons.close` to `FluentIcons.chrome_close`

## [3.6.1] - [27/12/2021]

- Fixed missing padding before close button on `TabView` ([#122](https://github.com/bdlukaa/fluent_ui/issues/122))
- Readded tab minimal size for `equal` and `sizeToContent` tab width behaviours ([#122](https://github.com/bdlukaa/fluent_ui/issues/122))
- `TabView`'s close button now uses `SmallIconButton`
- If a tab is partially off the view, it's scrolled until it's visible
- Fix `IconButton`'s icon size
- Update `OutlinedButton`, `FilledButton` and `TextButton` styles

## [3.6.0] - TabView Update - [25/12/2021]

- Implement `TreeView` ([#120](https://github.com/bdlukaa/fluent_ui/pull/120))
- Fix `Tooltip.useMousePosition`
- Fix `Slider` and `RatingBar` ([#116](https://github.com/bdlukaa/fluent_ui/issues/116))
- Fix scroll buttons when there are too many tabs in `TabView` ([#92](https://github.com/bdlukaa/fluent_ui/issues/92))
- Fix button style on tab in `TabView` ([#90](https://github.com/bdlukaa/fluent_ui/issues/90))
- Added *Close on middle click* on tabs in `TabView` ([#91](https://github.com/bdlukaa/fluent_ui/issues/91))
- Added `newTabLabel`, `closeTabLabel`, `scrollTabBackward`, `scrollTabForward` to `FluentLocalizations`
- Fix `TabView`'s text when it's too long. Now it's clipped when overflow and line doesn't break
- Added `TabView.closeButtonVisibility`. Defaults to `CloseButtonVisibilityMode.always`
- Updated selected tab paint
- Added `TabView.tabWidthBehavior`. Defaults to `TabWidthBehavior.equal`
- Added `TabView.header` and `TabView.footer`
- `Slider`'s mouse cursor is now [MouseCursor.defer]
- Added `SmallIconButton`, which makes an [IconButton] small if wrapped. It's used by `TextBox`
- Added `ButtonStyle.iconSize`
- **BREAKING** `AutoSuggestBox` updates:
  - Added `FluentLocalizations.noResultsFoundLabel`. "No results found" is the default text
  - Removed `itemBuilder`, `sorter`, `noResultsFound`, `textBoxBuilder`, `defaultNoResultsFound` and `defaultTextBoxBuilder`
  - Added `onChanged`, `trailingIcon`, `clearButtonEnabled` and `placeholder`
  - `controller` is now nullable. If null, an internal controller is creted

## [3.5.2] - [17/12/2021]

- **BREAKING** Removed `ThemeData.inputMouseCursor`
- **BREAKING** Removed `cursor` from `DatePicker`, `TimePicker`, `ButtonStyle`, `CheckboxThemeData`, `RadioButtonThemeData`, `SliderThemeData`, `ToggleSwitchThemeData`, `NavigationPaneThemeData`
- Scrollbar is not longer shown if `PaneDisplayMode` is `top`
- If open the compact pane, it's not always a overlay
- Added `triggerMode` and `enableFeedback` to `Tooltip`.
- Added `Tooltip.dismissAllToolTips`

## [3.5.1] - [15/12/2021]

- Update inputs colors
- `Expander` now properly disposes its resources
- Add the `borderRadius` and `shape` attributes to the `Mica` widget
- Implement `DropDownButton` ([#85](https://github.com/bdlukaa/fluent_ui/issues/85))

## [3.5.0] - Flutter 2.8 - [09/12/2021]

- **BREAKING** Minimal Flutter version is now 2.8
- `NavigationAppBar.backgroundColor` is now applied correctly. ([#100](https://github.com/bdlukaa/fluent_ui/issues/100))
- ComboBox's Popup Acrylic can now be disabled if wrapped in a `DisableAcrylic` ([#105](https://github.com/bdlukaa/fluent_ui/issues/105))
- `NavigationPane` width can now be customizable ([#99](https://github.com/bdlukaa/fluent_ui/issues/99)) 
- Implement `PaneItemAction` for `NavigationPane` ([#104](https://github.com/bdlukaa/fluent_ui/issues/104))

## [3.4.1] - [08/11/2021]

- `ContentDialog` constraints can now be customizable ([#86](https://github.com/bdlukaa/fluent_ui/issues/86))
- Add possibility to disable acrylic by wrapping it in a `DisableAcrylic` ([#89](https://github.com/bdlukaa/fluent_ui/issues/89))
- Fix `onReaorder null exception` ([#88](https://github.com/bdlukaa/fluent_ui/issues/88))
- Implement `InfoBadge`
- Implement `Expander` ([#85](https://github.com/bdlukaa/fluent_ui/issues/85))
- Default `inputMouseCursor` is now `MouseCursor.defer`
- `NavigationView.contentShape` is now rendered at the foreground

## [3.4.0] - Flexibility - [22/10/2021]

- `ProgressRing` now spins on the correct direction ([#83](https://github.com/bdlukaa/fluent_ui/issues/83))
- Added the `backwards` property to `ProgressRing`
- `FluentApp.builder` now works as expected ([#84](https://github.com/bdlukaa/fluent_ui/issues/84))
- Implemented `NavigationPane.customPane`, which now gives you the ability to create custom panes for `NavigationView`
- **BREAKING** `sizes`, `offsets` and `index` parameters from `NavigationIndicatorBuilder` were replaced by `pane`

## [3.3.0] - [12/10/2021]

- Back button now isn't forced when using top navigation mode ([#74](https://github.com/bdlukaa/fluent_ui/issues/74))
- `PilButtonBar` now accept 2 items ([#66](https://github.com/bdlukaa/fluent_ui/issues/66))
- Added builder variant to `NavigationBody`. 
- Fixed content bug when `AppBar` was not supplied too `NavigationView`

## [3.2.0] - Flutter 2.5.0 - [15/09/2021]

- Added missing parameters in `_FluentTextSelectionControls` methods ([#67](https://github.com/bdlukaa/fluent_ui/issues/67))
- Min Flutter version is now 2.5.0
- **EXAMPLE APP** Updated the url strategy on web.
- **EXAMPLE APP** Upgraded dependencies
- Format code according to flutter_lints

## [3.1.0] - Texts and Fixes - [25/08/2021]

- Updated Typography:
  - **BREAKING** Renamed `header` -> `display`
  - **BREAKING** Renamed `subHeader` -> `titleLarge`
  - **BREAKING** Renamed `base` -> `bodyStrong`
  - Added `bodyLarge`
  - Updated font size and weight for most of the text styles
- Update `SplitButton` design
- Update `IconButton` design
- Fixed `ToggleSwitch` not showing expanded thumb mode when dragging
- **BREAKING** Remove `CheckboxListTile`, `RadioListTile` and `SwitchListTile`. Use the respective widget with the `content` property

## [3.0.0] - Windows 11 - [24/08/2021]

- Update `ToggleButton` design.
- Update `Button` design.
- Update `RadioButton` design.
- Update `ContentDialog` design.
- Update `NavigationView` design:
  - **BREAKING:** Acryic is not used anymore. Consequently, `useAcrylic` method was removed.
- Implemented `Mica`, used by the new `NavigationView`
- Added support for horizontal tooltips. Set `Tooltip.displayHorizontally` to true to enable it.
- Updated Acrylic to support the web
- Update `Checkbox` design
- Update `ToggleSwitch` design
- Update `Scrollbar` design
- Update `Slider` design
- Update `InfoBar` design
- Update pickers design (`Combobox`, `DatePicker` and `TimePicker`)

## [2.2.1] - [26/06/2021]

- Implement Fluent Selection Controls for `TextBox` ([#49](https://github.com/bdlukaa/fluent_ui/pull/49))
- `Tooltip` is now displayed when focused ([#45](https://github.com/bdlukaa/fluent_ui/issues/45))
- AppBar is now displayed when minimal pane is open.
- AppBar's animation now follows the pane animation

## [2.2.0] - BREAKING CHANGES - [25/06/2021]

- **BREAKING:** Material `Icons` are not used anymore. Use `FluentIcons` instead.
- **BREAKING:** Reworked the `Acrylic` widget implementation ([#47](https://github.com/bdlukaa/fluent_ui/pull/47))
- **BREAKING:** Removed the `useAcrylic` property from `NavigationView`. Acrylic is now used by default.
- `PaneDisplayMode.compact` has now a width of 40, not 50.
- Removed `SizeTransition` from `TabView`.

## [2.1.1] - [03/06/2021]

- Option to set a default font family on the theme data (`ThemeData.fontFamily`)
- `indicatorBuilder` is correctly applied to the automatic display mode in `NavigationView`
- An overlay is open when the toggle button is pressed on the compact display mode ([#43](https://github.com/bdlukaa/fluent_ui/issues/43))

## [2.1.0] - Mobile Update - [01/06/2021]

- Implemented `BottomNavigation`
- Implemented `BottomSheet`
- Implemented `Chip`
- Implemented `Snackbar`
- Implemented `PillButtonBar`
- New buttons variations:
  - `FillButton`
  - `OutlinedButton`
  - `TextButton`

---

- `PaneItem`s' `build` method is now overridable. You can know customize how the items in `NavigationView` should look like by overriding the method.
- Fixed bug that navigation indicator was not showing on the first frame
- Fixed minimal tooltip not updating when closed the overlay
- **EXAMPLE APP:** Navigation indicator is now configurable on the `Settings` page

## [2.0.3] - [28/05/2021]

- Correctly apply items positions to pane indicators, regardless of external factors, such as navigation view app bar ([#41](https://github.com/bdlukaa/fluent_ui/issues/41))
- Improved `NavigationIndicator`s performance

## [2.0.2] - [23/05/2021]

- **BREAKING CHANGES:** Reworked the theme api ([#39](https://github.com/bdlukaa/fluent_ui/pull/39)):

  - Removed the theme extension (`context.theme`). Use `FluentTheme.of(context)` instead
  - `ButtonState` is now a class that can receive a value. It now allows lerping between values, making `AnimatedFluentTheme` possible.

    Here's an example of how to migrate your code:

    _Before_: `cursor: (_) => SystemMouseCursors.click,`\
    _Now_: `cursor: ButtonState.all(SystemMouseCursors.click),`

  - All theme datas and `AccentColor` have now a lerp method, in order to make `AnimatedFluentTheme` possible.
  - Implemented `AnimatedFluentTheme`, in order to replace `AnimateContainer`s all around the library
  - Dedicated theme for each theme data ([#37](https://github.com/bdlukaa/fluent_ui/issues/37)):
    - IconTheme
    - ButtonTheme
    - RadioButtonTheme
    - CheckboxTheme
    - FocusTheme
    - SplitButtonTheme
    - ToggleButtonTheme
    - ToggleSwitchTheme
    - NavigationPaneTheme
    - InfoBarTheme
    - TooltipTheme
    - DividerTheme
    - ScrollbarTheme
  - `DividerThemeData` now has `verticalMargin` and `horizontalMargin` instead of an axis callback.
  - Updated button colors.
  - Removed `animationDuration` and `animationCurve` from theme datas (except from `NavigationPaneThemeData`).
  - Renamed `copyWith` to `merge` on theme datas (except from `ThemeData`)
  - Fixed typo `standart` -> `standard`
  - Implement `AnimatedAcrylic`

## [2.0.1] - [21/05/2021]

- Minimal flutter version is now 2.2
- Implement `FluentScrollBehavior`, that automatically adds a scrollbar into listviews ([#35](https://github.com/bdlukaa/fluent_ui/pull/35))
- Reworked the inputs api ([#38](https://github.com/bdlukaa/fluent_ui/pull/38)):
  - A input can have multiple states. Now, if the widget is focused and pressed at the same time, it doesn't lose its focused border.
  - Now, the focus is not requested twice when the button is pressed, only once. This fixes a bug introduced in a previous version that combo boxes items we're not being focused.
  - Semantics (acessibility) is now applied on all inputs

## [2.0.0] - [20/05/2021]

- New way to disable the acrylic blur effect. Just wrap the acrylic widget in a `NoAcrylicBlurEffect` to have it disabled.
- Reworked the Navigation Panel from scratch ([#31](https://github.com/bdlukaa/fluent_ui/pull/31)):
  - The legacy `NavigationPanel` and `Scaffold` were removed. Use `NavigationView` and `ScaffoldPage` instead
  - Implemented open, compact, top and minimal display modes.
  - Custom Selected Indicators
- Implemented fluent localizations ([#30](https://github.com/bdlukaa/fluent_ui/issues/30))

## [1.10.1] - [05/05/2021]

- **FIX** Reworked the combo box widget to improve fidelity. ([#25](https://github.com/bdlukaa/fluent_ui/pull/25))
- **FIX** Improved `HoverButton` focus management.
- **FIX** Reworked the tooltip widget. Now, if any mouse is connected, the tooltip is displaying according to the pointer position, not to the child's. ([#26](https://github.com/bdlukaa/fluent_ui/pull/26))
- **FIX** TabView is now scrollable if the size of the tabs overflow the width

## [1.10.0] - **BREAKING CHANGES** - [03/05/2021]

- **BREAKING** `InfoHeader` was renamed to `InfoLabel`. You can now set if the label will be rendered above the child or on the side of it.
- **FIX** Fixed `RadioButton` inner color overlaping the border.
- **NEW** `ThemeData.inputMouseCursor`
- **FIDELITY** Switch thumb is now draggable. (Fixes [#22](https://github.com/bdlukaa/fluent_ui/issues/22))
- **EXAMPLE** Reworked the example app inputs page

## [1.9.4] - [02/05/2021]

- **FIX** `CheckboxListTile`, `SwitchListTile` and `RadioListTile` now doesn't focus its leading widget.
- **FIX** `TabView` is now not scrollable
- **FIX** Fixed `Acrylic` blur effect being disabled by default.
- **FIDELITY** Improved `ContentDialog` transition fidelity
- **FIX** Fixed `FocusBorder` for some widgets. It was affecting layout when it shouldn't
- **FIX** `RatingBar` and `Slider` weren't working due to `FocusBorder`
- **NEW** | **FIDELITY** New `Slider` thumb

## [1.9.3] - [01/05/2021]

- **NEW** `FocusBorder.renderOutside`. With this property, you can control if the FocusBorder will be rendered over the widget or outside of it.
- **FIX** Fixed `RadioButton`s border when focused
- **FIX** `Color.resolve` now doesn't throw a stack overflow error.
- **BREAKING** Removed `Color.resolveFromBrightness`. This is only available on `AccentColor`
- **EXAMPLE APP** Hability to change the app accent color
- **NEW** `darkest` and `lightest` colors variants in `AccentColor`
- **FIX** Fixed `InfoBar`'s error icon. It now uses `Icons.cancel_outlined` instead of `Icons.close`
- **NEW** `NavigationPanel` now has a `Scrollbar` and the `bottom` property is now properly styled if selected

## [1.9.2] - [30/04/2021]

- **FIX** `TabView` tabs can now be reordered (Fixes [#10](https://github.com/bdlukaa/fluent_ui/issues/10))
- **FIDELITY** If a new `Tab` is added, its now animated
- **FIX** `FocusBorder` now doesn't change the size of the widgets
- **BREAKING** `buttonCursor`, `uncheckedInputColor` and `checkedInputColor` are now moved to `ButtonThemeData` as static functions.

## [1.9.1] - [29/04/2021]

- **FIX** Fixed diagnostic tree. (Fixes [#17](https://github.com/bdlukaa/fluent_ui/issues/17))
- **FIX** | **FIDELITY** `TappableListTile` now changes its color when focused instead of having a border
- **FIDELITY** Improved `Acrylic`'s blur effect fidelity
- **FIX** `Acrylic`'s elevation was being applying margin
- **NEW** `ThemeData.shadowColor`, which is now used by `Acrylic`
- **NEW** You can now globally disable the acrylic blur effect by changing `Acrylic.acrylicEnabled`

## [1.9.0] - **BREAKING CHANGES** - Theme Update - [29/04/2021]

The whole theme implementation was reworked on this change.

- **BREAKING** Renamed `Theme` to `FluentTheme`
- **BREAKING** All the properties in `FluentTheme` now can't be null
- **BREAKING** Renamed all the `Style` occurrences to `ThemeData`
- **BREAKING** `ThemeData.accentColor` is now an `AccentColor`
- **FIX** When providing a custom style to a tooltip, it's now correctly applied to `ThemeData.tooltipStyle`
- **FIX** `debugCheckHasFluentTheme` has now a better error message
- **FIX** `FluentApp` now doesn't throw an error if no `theme` is provided
- **FIX** Reworked `Scrollbar` to improve fidelity.
- **NEW** Color extension methods: `Color.toAccentColor` and `Color.basedOnLuminance`
- **NEW** `Button.builder`

## [1.8.1] - [16/04/2021]

- **NEW** In `TabView`, it's now possible use the following shortcuts if `TabView.shortcutsEnabled` is `true` (Follows [this](https://docs.microsoft.com/en-us/windows/uwp/design/controls-and-patterns/tab-view#closing-a-tab)):
  1. `Ctrl + F4` or `Ctrl + W` to close the current tab
  2. `Ctrl + T` to create a new tab
  3. `1-8` to navigate to a tab with the pressed number
  4. `9` to navigate to the last tab and navigate to the last tab
- **NEW** `IconButton.autofocus`, `ToggleButton.autofocus`
- **BREAKING** Renamed all the `semanticsLabel` to `semanticLabel`

## [1.8.0] - Color Update - [14/04/2021]

- **NEW** Web version hosted at https://bdlukaa.github.io/fluent_ui
- **NEW** Colors showcase page in example app
- **NEW** Info Colors:
  - `Colors.warningPrimaryColor`
  - `Colors.warningSecondaryColor`
  - `Colors.errorPrimaryColor`
  - `Colors.errorSecondaryColor`
  - `Colors.successPrimaryColor`
  - `Colors.successSecondaryColor`
- **FIX** Reworked all the accent colors (`Colors.accentColors`) with `darkest`, `dark`, `normal`, `light` and `lighter`
- **BREAKING** `Colors.blue` is now an `AccentColor`

## [1.7.6] - [13/04/2021]

- **NEW** `Checkbox.autofocus`
- **BREAKING** `Button` refactor:
  - Removed `Button.icon` and `Button.trailingIcon`
  - Renamed `Button.text` to `Button.child`
- You can now disable the acrylic backdrop effect by setting `enabled` to false
- **NEW** `NavigationPanelBody.animationCurve` and `NavigationPanelBody.animationDuration`

## [1.7.5] - [13/04/2021]

- **NEW** `Scrollbar` and `ScrollbarStyle`
- Reworked `FluentApp` to not depend of material anymore.

## [1.7.4] - [10/04/2021]

- **FIX** Updated `Icon` widget to use Flutter's default icon widget
- **NEW** Documentation

## [1.7.3] - [07/04/2021]

- **FIX** Improved `ListTile` sizing ([#Spacing](https://docs.microsoft.com/en-us/windows/uwp/design/style/spacing))
- **NEW** `FocusStyle` and support for glow focus
- **NEW** `RatingBar.starSpacing`

## [1.7.2] - [06/04/2021]

- **FIX** Animation when using `NavigationPanelBody` now works as expected
- **NEW** `CheckboxListTile`, `SwitchListTile` and `RadioListTile`
- **FIX** It's now not possible to focus a disabled `TextBox`

## [1.7.1] - [06/04/2021]

- **FIX** The mouse cursor in a disabled input is now `basic` instead of `forbidden`
- **FIX** `NavigationPanelBody` now doesn't use a `IndexedStack` under the hood because it was interfering in the focus scope
- **FIX** The color of the focus now is the `Style.inactiveColor`
- **FIX** `RadioButton`'s cursor was not being applied correctly
- **NEW** `Button.toggle`
- **FIX** The state provided by `HoverButton` was being `focused` when it shouldn't be
- **FIX** TimePicker showing wrong minute count. It should start from 00 and end in 59
- **NEW** `TimePicker.minuteIncrement`

## [1.7.0] - Focus Update - [05/04/2021]

- **FIXED** Fixed the possibility to give a elevation lower than 0 in `Acrylic`
- **NEW** It's now possible to change the rating of `RatingBar` using the keyboard arrows
- **NEW** Now it's possible to navigate using the keyboard with all focusable widgets

## [1.6.0] - BREAKING CHANGES - [03/04/2021]

- Added the missing `Diagnostics`
- Updated all the screenshots
- **BREAKING CHANGE** Uses the material icon library now

  **DEVELOPER NOTE** This was a hard choice, but the material icon library is a robust, bigger library. It contains all the icons the previous library has, and a few many more.

## [1.5.0] - [02/04/2021]

- Added `Diagnostics` to many widgets
- **NEW** `AutoSuggestBox` (Follows [this](https://docs.microsoft.com/en-us/windows/uwp/design/controls-and-patterns/auto-suggest-box))
- **NEW** `Flyout` and `FlyoutContent` (Folllows [this](https://docs.microsoft.com/en-us/windows/uwp/design/controls-and-patterns/dialogs-and-flyouts/flyouts))
- **FIXED** Popup was being shown off-screen.

  **DEVELOPER NOTE** The solution for this was to make it act like a tooltip: only show the popup above or under the `child`. This was a hard choice, but the only viable option that would work on small screens/devices. This also made `Flyout` easier to implement. This should be changed when multi-window support is available.

- **FIXED** `DatePicker` incorrectly changing hour
- **NEW** `Colors.accentColors`
- Documentation about [system_theme](https://pub.dev/packages/system_theme)
- **BREAKING** Removed `Pivot` because it's deprecated

## [1.4.1] - Pickers Update - [30/03/2021]

- **NEW** `Style.fasterAnimationDuration`
- **FIX** `ComboBox` press effect
- **NEW** `TimePicker` (Follows [this](https://docs.microsoft.com/en-us/windows/uwp/design/controls-and-patterns/time-picker))
- **NEW** `DatePicker` (Follows [this](https://docs.microsoft.com/en-us/windows/uwp/design/controls-and-patterns/date-picker))

## [1.4.0] - [28/03/2021]

- **NEW** `InfoHeader`
- **NEW** `ComboBox` (Follows [this](https://docs.microsoft.com/en-us/windows/uwp/design/controls-and-patterns/checkbox))
- **NEW** `TappableListTile`
- **BREAKING** Removed `DropdownButton` and `Button.dropdown`

## [1.3.4] - [28/03/2021]

- **NEW** Vertical Slider

## [1.3.3] - [25/03/2021]

- **NEW** Indeterminate `ProgressRing` ([@raitonoberu](https://github.com/raitonoberu))
- **NEW** `ListTile`
- **DIAGNOSTICS** Provide `Diagnostics` support to:
  - `Style`
  - `NavigationPanelStyle`
  - `TooltipStyle`

## [1.3.2] - Accessibility update - [24/03/2021]

This version provides the fix for [#5](https://github.com/bdlukaa/fluent_ui/issues/5)

- `Theme.of` can't be null anymore. Use `Theme.maybeOf` for such
- **NEW** `Style.inactiveBackgroundColor`
- **BREAKING** Replaced `color`, `border`, `borderRadius` from `IconButtonStyle` to `decoration`
- **DIAGNOSTICS** Provide `Diagnostics` support to the following classes:
  - ButtonStyle
  - Checkbox
  - CheckboxStyle
  - IconButtonStyle
  - RadioButtonStyle
  - RatingBar
  - SplitButtonStyle
  - ToggleButton
  - ToggleButtonStyle
  - ToggleSwitch
  - ToggleSwitchStyle
  - Slider
  - SliderStyle
  - Typography
  - Divider
  - DividerStyle
- Provide accessibility support to the following widgets:
  - Button
  - Checkbox
  - IconButton
  - RadioButton
  - RatingBar
  - Slider
  - ToggleButton
  - ToggleSwitch
  - TabView

## [1.3.1] - [23/03/2021]

- **FIX** `IconButtonStyle`'s `iconStyle` now works properly
- Improved `TabView` icon styling
- **NEW** Indeterminate `ProgressBar` ([@raitonoberu](https://github.com/raitonoberu))

## [1.3.0] - [22/03/2021]

- **NEW** Determinate `ProgressBar` and `ProgressRing`
- **NEW** `TabView` ([#TabView](https://docs.microsoft.com/en-us/windows/uwp/design/controls-and-patterns/tab-view))

## [1.2.5] - [21/03/2021]

- **FIX** Fixed `InfoBar`'s overflow

## [1.2.4] - [21/03/2021]

- **BREAKING** `RadioButton`'s `selected` property was renamed to `checked` to match a single pattern between all the other widgets.

## [1.2.3] - [19/03/2021]

- **NEW** | **EXAMPLE APP** `Settings` screen
- Improved theme changing
- **FIX** `FluentApp` doesn't lose its state anymore, possibiliting hot relaod.
- **NEW** `showDialog` rework:
  - `showDialog` now can return data. (Fixes [#2](https://github.com/bdlukaa/fluent_ui/issues/2))
  - `showDialog.transitionBuilder`
  - `showDialog.useRootNavigator`
  - `showDialog.routeSettings`
  - It's no longer necessary to have the fluent theme to display dialogs using this function.

## [1.2.2] - [17/03/2021]

- **BREAKING** Removed `_regular` from the name of the icons.
- **NEW** `InfoBar` (Follows [this](https://docs.microsoft.com/en-us/windows/uwp/design/controls-and-patterns/infobar))

## [1.2.1] - [16/03/2021]

- **NEW** `Divider`

## [1.2.0] - Timing and easing - Page transitioning - [15/03/2021]

- **FIDELITY** Improved `ToggleButton` fidelity
- **NEW** `NavigationPanelBody`
- **NEW** Page transitions
  - `EntrancePageTransition` ([#PageRefresh](https://docs.microsoft.com/en-us/windows/uwp/design/motion/page-transitions#page-refresh))
  - `DrillInPageTransition` ([#Drill](https://docs.microsoft.com/en-us/windows/uwp/design/motion/page-transitions#drill))
  - `HorizontalSlidePageTransition` ([#HorizontalSlide](https://docs.microsoft.com/en-us/windows/uwp/design/motion/page-transitions#horizontal-slide))
  - `SuppressPageTransition` ([#Supress](https://docs.microsoft.com/en-us/windows/uwp/design/motion/page-transitions#suppress))
- Add timing and easing to style. (Follows [this](https://docs.microsoft.com/en-us/windows/uwp/design/motion/timing-and-easing))
  - **NEW** `Style.fastAnimationDuration` (Defaults to 150ms)
  - **NEW** `Style.mediumAnimationDuration` (Defaults to 300ms)
  - **NEW** `Style.slowAnimationDuration` (Defaults to 500ms)
  - Default `animationCurve` is now `Curves.easeInOut` (standard) instead of `Curves.linear`
  - **BREAKING** Removed `Style.animationDuration`
- Refactored Navigation Panel

## [1.1.0] - Fidelity update - [14/03/2021]

- **BREAKING** Removed `Card` widget. Use `Acrylic` instead
- **NEW** `Acrylic` widget ([#Acrylic](https://docs.microsoft.com/en-us/windows/uwp/design/style/acrylic))
- **NEW** **NAVIGATION PANEL** `bottom` property
- **FIDELITY** Improved the corder radius of some widgets (Follows [this](https://docs.microsoft.com/en-us/windows/uwp/design/style/rounded-corner#page-or-app-wide-cornerradius-changes))
- **FIX** **FIDELITY** Dark theme hovering color
- Improved documentation

## [1.0.2] - Typography update - [11/03/2021]

- **NEW** Typography
  - Migrated all the widgets to use typography
- **NEW** Tooltip
- **NEW** Dark theme
- **FIX** Disabled button press effect if disabled
- **FIX** Grey color resulting in green color

## [1.0.1+1] - [09/03/2021]

- **NEW** Screenshots

## [1.0.1] - [07/03/2021]

- **FIX** `NavigationPanel` navigation index
- **FIX** `Slider`'s inactive color
- **FIDELITY** Scale animation of button press
- **FIDELITY** Improved `Slider` label fidelity
- **NEW** Split Button

## [1.0.0] - [05/03/2021]

- **NEW** Null-safety
- **NEW** New Icons Library
- **NEW** `NavigationPanelSectionHeader` and `NavigationPanelTileSeparator`
- **BREAKING** Removed `Snackbar`

## [0.0.9] - [03/03/2021]

- Export the icons library
- **NEW** `TextBox`

## [0.0.8] - [01/03/2021]

- **NEW** `ContentDialog` 🎉
- **NEW** `RatingControl` 🎉
- **NEW** `NavigationPanel` 🎉
- Improved `Button` fidelity

## [0.0.7] - [28/02/2021]

- **NEW** `Slider` 🎉
- Use physical model for elevation instead of box shadows
- Improved TODO

## [0.0.6] - [27/02/2021]

- **FIXED** Button now detect pressing
- **FIXED** `ToggleSwitch` default thumb is now animated
- **FIXED** Improved `ToggleSwitch` fidelity
  **FIXED** Darker color for button press.
- **NEW** **THEMING**
  - `Style.activeColor`
  - `Style.inactiveColor`
  - `Style.disabledColor`
  - `Style.animationDuration`
  - `Style.animationCurve`

## [0.0.5] - [27/02/2021]

- `ToggleSwitch` is now stable 🎉
- **NEW** `DefaultToggleSwitchThumb`
- **NEW** `ToggleButton`
- New toast lib: [fl_toast](https://pub.dev/packages/fl_toast)
- Screenshot on the readme. (Fixes [#1](https://github.com/bdlukaa/fluent_ui/issues/1))

## [0.0.4] - [22/02/2021]

- New fluent icons library: [fluentui_icons](https://pub.dev/packages/fluentui_icons)
- Re-made checkbox with more fidelity
- Refactored the following widgets to follow the theme accent color:
  - `Checkbox`
  - `ToggleSwitch`
  - `RadioButton`
- Added accent colors to widget. Use [this](https://docs.microsoft.com/en-us/windows/uwp/design/style/images/color/windows-controls.svg) as a base

## [0.0.3] - Theming update - [21/02/2021]

- **HIGHLIGHT** A whole new [documentation](https://github.com/bdlukaa/fluent_ui/wiki)
- Scaffold now works as expected.
- Improved theming checking
- **NEW**
  - `null` (thirdstate) design on `Checkbox`. (Follows [this](https://docs.microsoft.com/en-us/windows/uwp/design/controls-and-patterns/checkbox))
  - Now you can use the `Decoration` to style the inputs
- **BREAKING**:
  - Removed `Button.action`
  - Removed `Button.compound`
  - Removed `Button.primary`
  - Removed `Button.contextual`
  - Removed `AppBar`
  - Now the default theme uses accent color instead of a predefined color (Follows [this](https://docs.microsoft.com/en-us/windows/uwp/design/style/color#accent-color))
- **FIXED**:
  - `ToggleSwitch` can NOT receive null values

## [0.0.2] - [18/02/2021]

- The whole library was rewritten following [this](https://docs.microsoft.com/en-us/windows/uwp/design/)
- Tooltip's background color is now opaque (Follows [this](https://docs.microsoft.com/en-us/windows/uwp/design/controls-and-patterns/tooltips))
- Dropdown button now works as expected
- **FIXED**:
  - Snackbar now is dismissed even if pressing or hovering
  - Margin is no longer used as part of the clickable button
- **BREAKING**:
  - Renamed `Toggle` to `ToggleSwitch` (Follows [this](https://docs.microsoft.com/en-us/windows/uwp/design/controls-and-patterns/toggles))
  - Removed `BottomNavigationBar`. It's recommended to use top navigation (pivots)
  - Removed `IconButton.menu`
- **NEW**:
  - NavigationPanel (Follows [this](https://docs.microsoft.com/en-us/windows/uwp/design/layout/page-layout#left-nav))
  - Windows project on example
  - RadioButton (Follows [this](https://docs.microsoft.com/en-us/windows/uwp/design/controls-and-patterns/radio-button))

## [0.0.1]

- Initial release
