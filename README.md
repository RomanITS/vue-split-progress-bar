# vue2-progress-bar
ProgressBar for vue.js <br>
SVG/Vector based <br>
4 modes: _Line_, _Circle_, _Cylinder_ and _Battery_ <br>
v1.0.0

[Live demo](http://softwarefun.no/#/progressbar)

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
data: [
  {
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
  },
  {
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
  },
  {
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
  },
  {
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
  },
],
```

### Properties
Standard Style Array
  styles: ['low', 'middle', 'high', 'none'],

Tooltip Visibility Control
  showInfo: false,

Percent value for tooltip
  percent: '',

Hint Quantity Value
  value: '',

The meaning of the name for the tooltip
  name: '',

Tooltip Style Value
  style: '',

Variable for custom styles of the progress bar
  customStyle: {}
}
| Name            | Type    | Default           | Description                        |
| ---             | ---     | ---               | ---                                |
| value           | Number  | 0                 | Значение количества для подсказки  |
| styles          | Array   | ['low', 'middle', | Стандартный массив стилей          |
|                 |         | 'high', 'none']   |                                    |
| showInfo        | Boolean | false             | Контроль видимости подсказки       |
| percent         | String  | ''                | Значение процентов для подсказки   |
| name            | String  | ''                | Значение названия для подсказки    |
| style           | String  | ''                | Значение стиля для подсказки       |
| customStyle     | Object  | {}                | Переменная для пользовательских    |
|                 |         |                   | стилей progress bar                |

