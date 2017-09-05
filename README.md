# rn

## Components
* https://github.com/react-native-training/react-native-elements
* [List Popover](https://github.com/bulenttastan/react-native-list-popover)
* [Scroll ScrollView inside a View](https://stackoverflow.com/a/38137781/6630464)

## Network
* [Fetch instead of Axios](https://www.udemy.com/the-complete-react-native-and-redux-course/learn/v4/questions/1924782)

## IDE (THE MOST PAINFUL PART OF THE JOURNEY)
* [Microsoft NIC Reprioritization](https://answers.microsoft.com/en-us/windows/forum/windows_10-networking/adapter-priority-setting-unavailable-in-windows-10/d2b63caa-e77c-4b46-88b5-eeeaee00c306?auth=1)
* [Github Issue about Microsoft NIC prioritization](https://github.com/react-community/create-react-native-app/issues/60#issuecomment-287081523)
* [Github Issue about Expo and multiple NICs](https://github.com/react-community/create-react-native-app/issues/81)
* [Setting ENV variable for NIC to listen to](https://github.com/react-community/create-react-native-app/blob/d01ddabb634532200629c6d17f920eb856fa6416/react-native-scripts/template/README.md#configuring-packager-ip-address)
* [Expo listens to the first NIC detected](https://github.com/react-community/create-react-native-app/issues/264#issuecomment-309525762)
* Development server has returned error 500.
    * Remove `yarn.lock` or `package-lock.json` and `node_modules/` then reinstall everything using `npm i` or `yarn`.
* How to style react-navigation default header?
```
static navigationOptions() {
  return {
    headerStyle: {backgroundColor: 'red'}
  }
}
```
* How to detect platform: Android vs IOS?
```
import {Platform} from 'react-native'
Platform.OS === 'android'
Platform.OS === 'ios'
```
## Deployment
### Android
- [ ] `package` - package name for the Android app. Usually in Reverse DNS notation e.g. "com.mydom.mysubdom"
- [ ] `versionCode` - integer from 1 to 2100000000. Prevents downgrade of users' apps.
- [ ] `icon` - 512x512 `.png` file that will appear in a device's home screen
- [ ] `permissions` - List of permissions.
- [ ] `config`
    - [ ] `branch` - branch.io configuration
    - [ ] `fabric`
    - [ ] `googleMaps`
    - [ ] `googleSignIn`
- [ ] `facebookScheme`
- [ ] `hooks`
### IOS
