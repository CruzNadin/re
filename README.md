# CruzNadin Datepicker 


## ⚡ Npm Commands

Talk to us about more commands if you need

![visitors](https://visitor-badge.glitch.me/badge?page_id=react-native-cn-datepicker)

⚡ **Install**
  
```bash
npm i react-native-cn-datepicker
```
or
```bash
yarn add react-native-cn-datepicker
```

⚡ **npm run pod**

```bash
npx pod-install ios
```

![android](http://xgfe.github.io/react-native-datepicker/img/react-native-datepicker-android.gif)
![ios](http://xgfe.github.io/react-native-datepicker/img/react-native-datepicker-ios.gif)

⚡ **Usage**
  
```javascript

import DatePicker from 'react-native-cn-datepicker'

  render(){
    return (
      <DatePicker
        style={{width: '100%'}}
        date={this.state.date}
        mode="date"
        placeholder="select date"
        format="DD-MM-YYYY"
        display="spinner"
        is24Hour={false}
        confirmBtnText="Confirm"
        cancelBtnText="Cancel"
        customStyles={{
          placeholderText: {
            fontSize: 18,
            color: "#48515B"
          },
          dateText:{
            fontSize: 18
          },
          dateInput: {
            marginLeft: 36
          }
        }}
        onDateChange={(date) => {
            console.log(date);
        }}
        locale={"en"} // Default en
      />
    )
  }
}
```
⚡ **Properties**
    | Prop  | Default  | Type | Description |
| :------------ |:---------------:| :---------------:| :-----|
| style | - | `object` | Specify the style of the DatePicker, eg. width, height...  |
| date | - | <code>string &#124; date &#124; Moment instance</code> | Specify the display date of DatePicker. `string` type value must match the specified format |
| mode | 'date' | `enum` | The `enum` of `date`, `datetime` and `time` |
| androidMode | 'default' | `enum` | The `enum` of `default`, `calendar` and `spinner` (only Android) |
| format | 'YYYY-MM-DD' | `string` | Specify the display format of the date, which using [moment.js](http://momentjs.com/). The default value change according to the mode. |
| confirmBtnText | 'Confirm' | `string` | Specify the text of confirm btn in ios. |
| cancelBtnText | 'Cancel' | `string` | Specify the text of cancel btn in ios. |
| duration | 300 | `number` | Specify the animation duration of datepicker.|
| customStyles | - | `object` | The hook of customize datepicker style, same as the native style. `dateTouchBody`, `dateInput`...|
| hideText | false | `boolean` | Controller whether or not show the `dateText` |
| minDate | - | `string | date` | Restricts the range of possible date values. |
| maxDate | - | `string | date	` | Restricts the range of possible date values. |
| disabled | false | `boolean` | Controller whether or not disable the picker |
| is24Hour | - | `boolean` | Set the TimePicker is24Hour flag. The default value depend on `format`. Only work in Android |
| allowFontScaling | true | `boolean` | Set to false to disable font scaling for every text component |
| placeholder | '' | `string` | The placeholder show when this.props.date is falsy |
| onDateChange | - | `function` | This is called when the user confirm the picked date or time in the UI. The first and only argument is a date or time string representing the new date and time formatted by [moment.js](http://momentjs.com/) with the given format property. |
| onOpenModal | - | `function` | This is called when the DatePicker Modal open. |
| onCloseModal | - | `function` | This is called when the DatePicker Modal close |
| onPressMask | - | `function` | This is called when clicking the ios modal mask |
| modalOnResponderTerminationRequest | - | `function` | Set the callback for React Native's [Gesture Responder System](https://facebook.github.io/react-native/docs/gesture-responder-system.html#responder-lifecycle)'s call to `onResponderTerminationRequest`. By default this will reject a termination request, but can be overidden in case the View under the Modal is implementing custom gesture responders, and you wish for those to be overidden in certain cases.  |
| TouchableComponent | `TouchableHighlight` | `Component` | Replace the `TouchableHighlight` with a custom `Component`. For example : `TouchableOpacity` |
| getDateStr | - | Function | A function to override how to format the date into a `String` for display, receives a `Date` instance

## 📫 Contact Us

- Email - [info@tulparyazilim.com.tr](mailto:info@tulparyazilim.com.tr)
- LinkedIn - [Tulpar Yazılım](https://www.linkedin.com/company/tulparyazilim)
- Blog - [Blog](https://www.tulparyazilim.com.tr/blog)

---

<img src="https://www.tulparyazilim.com.tr/img/logo.png" />

⭐️ From [Tulpar Yazılım](https://github.com/tulparyazilim)
