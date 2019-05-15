# react-native-intro
A way for new  feature introduction and step-by-step users guide for your react-native app

# Install

add "react-native-intro": "git+https://github.com/ylnjuuju/react-native-intro.git" to package.json file and npm install

# Usage

1. react-native-intro exports two APIs, default is ```Intro``` component, and the other one is ```intro``` function. see [demo](./demo/) get more informations.

2. Use ```Intro``` component wrap your components and pass some props to Intro. Maybe you need set the style props too;

```
import Intro, {IntroManage} from 'react-native-intro';
// collapsable make sure android measure method can get value
<Intro
    content={"hello world"}
    step={1}>
    collapsable={false}
</Intro>

.....

componentDidMount() {

    // and start
    var myIntro = new IntroManage();
    myIntro.start();

}

```

#Props
###content: string | ReactElement

###step: the step sort

# Warning
 *This Component does not support your component Wrapped by `Redux connect` currently;*

# screen shorts

![ios screen shoot](./demo/ios.gif)
![android screen shoot](./demo/android.gif)
