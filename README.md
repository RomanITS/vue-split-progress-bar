# vue2-progress-bar
ProgressBar for vue.js
SVG/Vector based
4 modes: _Line_, _Circle_, _Cylinder_ and _Battery_
v1.0.0

Do you have questions or want a new feature? Use the "Issues" section :point_left:

## Setup
install:
```bash
npm install vue2-progress-bar --save
```

Import: (in your main.js)
```javascript
import ProgressBar from 'vue2-progress-bar'
Vue.use(ProgressBar)
```
## Usage
Use: (in your local .vue file/component, html section)

```xml
<progress-bar
  :label="data.label"
  :max="200"
  :data="data.elementData"
/>
```
```javascript
// variant 1
data: {
  label: "Risk of Loss",
  elementData: [
    {
      style: "low",
      name: "Low",
      value: 1,
    },
    {
      style: "middle",
      name: "Middle",
      value: 78,
    },
    {
      style: "high",
      name: "High",
      value: 120,
    },
  ],
}
// variant 2
data: {
  label: "Satisfaction",
  elementData: [
    {
      style: "low",
      name: "Low",
      value: 1,
    },
    {
      style: "middle",
      name: "Middle",
      value: 8,
    },
    {
      style: "high",
      name: "High",
      value: 10,
    },
  ],
}
// variant 3
data: {
  label: "Impact of Loss",
  elementData: [
    {
      style: "low",
      name: "Low",
      value: 40,
    },
    {
      style: "middle",
      name: "Middle",
      value: 144,
    },
    {
      style: "high",
      name: "High",
      value: 16,
    },
  ],
}
// variant 4
data: {
  elementData: [
    {
      style: "low",
      name: "Low",
      value: 140,
    },
    {
      style: "#bee5eb",
      name: "Middle",
      value: 40,
    },
    {
      style: "",
      name: "High",
      value: 16,
    },
  ],
}
```

### Props
| Name     | Type   | Required    | Default     | Description                       |
| ---      | ---    | ---         | ---         |  ---                              |
| data     | Object | true        | null        | Data to fill in the progress bar  |
| label    | String | false       | ''          | Title progress                    |
| max      | Number | false       | 100         | The maximum progress value        |

### Properties
| Name            | Type    | Default           | Description                             |
| ---             | ---     | ---               | ---                                     |
| value           | Number  | 0                 | Hint Quantity Value                     |
| styles          | Array   | ['low', 'middle', 'high', 'none'] | Standard Style Array    |
| showInfo        | Boolean | false             | Tooltip Visibility Control              |
| percent         | String  | ''                | Percent value for tooltip               |
| name            | String  | ''                | The meaning of the name for the tooltip |
| style           | String  | ''                | Tooltip Style Value                     |
| customStyle     | Object  | {}                | Variable for custom styles of the progress bar |

