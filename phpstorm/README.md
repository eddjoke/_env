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

## ESLint autofix and current file linting

Eslint shows warnings and errors when code is not well formatted. You can initiate autofixing command to fix the issues for you!
Full tutorial here: https://blog.jetbrains.com/webstorm/2016/08/using-external-tools/

First, you need to set an external tool and then set a shortcut to call it.

1: Set an external tool: ![image](/images/eslint-as-external-tool-setup.png)

```
ESLint fix
Automatically fix issue with locally installed ESLint

./node_modules/.bin/eslint
--fix --color $FilePathRelativeToProjectRoot$
$ProjectFileDir$
```

and

```
ESLint
Lint the current file with locally installed ESLint

./node_modules/.bin/eslint
--color $FilePathRelativeToProjectRoot$
$ProjectFileDi]$
```

2: Set a shortcut for external tool: ![image](/images/eslint-shortcut-setup.png)

I have set it to my personal shortcut `Ctrl+Alt+L` to lint the code and `Ctrl+Alt+F` to fix the code.

P.s. Macro can be created and shortcut can be set to "Autofix and save" if necessary.

#### Note: ESlint takes locally installed package, so linters will not work if you don't have eslint package under node_modules.
