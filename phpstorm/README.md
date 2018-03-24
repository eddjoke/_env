# PhpStorm

## Plugins

Install downloading with link or searching by name in PhpStorm (**Preferences** > **Plugins** > **Install Jetbrains plugin...**)

* [EditorConfig](https://plugins.jetbrains.com/plugin/7294-editorconfig)
* [PostCSS support](https://plugins.jetbrains.com/plugin/8578-postcss-support)
* [.ignore](https://plugins.jetbrains.com/plugin/7495--ignore)

## Live Templates

The following templates may be helpful when developing with PhpStorm. Add them to your editor as live templates (**Preferences** (`cmd + ,`) > **Editor** > **Live Templates**).

### **rfc** (react functional component)

```
import React from 'react';
import PropTypes from 'prop-types';

const $COMPONENT$ = ({$PROPS$}) => (
  <div>

  </div>
);

$COMPONENT$.propTypes = {
  $PROPTYPES$
};

$COMPONENT$.defaultProps = {
  // empty for now
};

export default $COMPONENT$;
```

---

### **rcc** (react class component):

```
import React from 'react';
import PropTypes from 'prop-types';

class $COMPONENT$ extends React.Component {
  render() {
    const { $PROPS$ } = this.props;
    return (
      <div>
        $CONTENT$
      </div>
    );
  }
}

$COMPONENT$.propTypes = {

};

export default $COMPONENT$;
```

---

### **fn** (general JavaScript function)

```
function $FUNCTION_NAME$($PARAMS$) {
  return $RESULT$;
}
```

---

### **fna** (ES6 arrow function)

```
const $FUNCTION_NAME$ = ($PARAMS$) => $RESULT$;
```
