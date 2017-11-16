<center>
<h1>👟 React Scroll-To</h1>
</center>
<hr />

A render prop component that allows child components to trigger scrolling to a window position.

### Install

**npm:** `npm install react-scroll-to --save`

**yarn:** `yarn add react-scroll-to`


### Example

```
import React, { Component } from "react";
import { ScrollTo} from "react-scroll-to";

export default class MyComponent extends React {
    render() {
        return (
            <ScrollTo>
                {
                    (onScroll) => (
                        <a onClick={onScroll(0, 500)}>
                            Scroll to Bottom
                        </a>
                    ) 
                }
            </ScrollTo>
        );
    }
}
```
