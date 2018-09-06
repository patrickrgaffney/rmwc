# Checkboxes

> Checkboxes allow the user to select multiple options from a set.

- import from **rmwc/Checkbox**  
- import styles from **@material/checkbox/dist/mdc.checkbox.css**
- [https://material.io/develop/web/components/input-controls/checkboxes/](https://material.io/develop/web/components/input-controls/checkboxes/)

```jsx render
import { Checkbox } from 'rmwc/Checkbox';

{/* Controlled with change handlers */}
<Checkbox
  checked={this.state.cookiesChecked || false}
  onChange={evt => this.setState({cookiesChecked: evt.target.checked})}>
  Cookies
</Checkbox>

{/* Standard Checkbox */}
<Checkbox>Pizza</Checkbox>

{/* Using the label prop */}
<Checkbox label="Icecream" />

{/* Making a "half" checked, indeterminate Checkbox */}
<Checkbox indeterminate={true}>Broccoli</Checkbox>
```

```jsx renderOnly
import { DocumentComponent } from 'rmwc/Base/utils/DocumentComponent';

<DocumentComponent displayName="Checkbox" />
```