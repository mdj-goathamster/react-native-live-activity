# dsb-react-native-live-activity

This is an example of a Native Module to control the iOS Live Activities.

## Installation

```sh

npm install dsb-react-native-live-activity

```

## Usage

```js
import {
startActivity,
listAllActivities,
endActivity,
updateActivity,
} from 'dsb-react-native-live-activity';


await startActivity("Packing", "Jhon", "12 PM")
await updateActivity(activity.id, "Driving", "Jhon", "12 PM");
await endActivity(activity.id);

const [activities, setActivities] = React.useState<any[]>([]);
listAllActivities().then(setActivities);

```

## Example

Run

```bash
$ yarn install
```

Then

```bash
$ open ./example/ios/LiveActivityExample.xcworkspace
```

After that build the xCode project.



https://user-images.githubusercontent.com/3778297/192741742-9d3a9bc5-e26a-4197-b152-5f60796736eb.mp4


## License

MIT

---

Made with [create-react-native-library](https://github.com/callstack/react-native-builder-bob)
